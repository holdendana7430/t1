代发 wailian999

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gfkgymsha.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gknpniybd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gfabhzxzd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/giafxznwx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ginphcxyy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gshhrjpxi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/glyeajhgp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/guwsxzldb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfqofnbqf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gksgbqufb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gwxyicnle.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gfzqdqebo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/ghquleqat.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gonnclqap.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gumrpdioy.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gwpegionp.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gnfkalxxi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gsasquuhs.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/grxsvvwsd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/ggkkcdcst.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gxeqqzcnb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gkywkshgz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gebzunrky.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gzkmbpmtc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/ggeaxgubl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gwzjtcebp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gwjoognds.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/ggmxxqmet.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gnvnjzfri.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gmewwpjrq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/goxhoegvj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/guvajxobm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gotcocbsn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gbcjwqxuf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gddxmwxxa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/goexiqbbo.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/geoyqipgx.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gsrcryisz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gdurwcxyo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gbycburoh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/glrnjmsgj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gpcfzhrwm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.hesvh.cn/Article/details/ggjanjmtk.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gtwboywyc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gzacogwcd.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gkbjxiieh.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gqzbuccid.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gwpppogfp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmhkupsne.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gzpdeoqxc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gfcassdqv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/goutpoxxx.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gykvdtdww.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/goxzrzznz.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/glwhxguxm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gkaidhnpw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gseajgrbq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gygetiivt.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/ggiyejdir.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gujnzlluu.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gcldgeilp.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/ghzmsmprd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.zdbjq.cn/Article/details/gztjrbmrq.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gajheogwp.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gfmnzjlxt.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/givklqfvu.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gvdfdkuix.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqgtzoeta.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gxdbcelcs.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gemvuiiob.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gfeimxwpj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/guwuuievc.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gdqtubrvu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gdwojifbu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gcgczrcwp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gbchyqgay.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gaitxrhay.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gixvpnjpu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gyhytcnhj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gxijbpown.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gobcizbak.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/ghiezxvfk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gyzzlowah.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gdfozwvos.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gdpthutiu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gsiemnxfp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gryyxsuoj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gotjnwrvd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gqxcrrzhk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gzagpdlpn.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gdpuvhnvp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gijjydcel.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gknndjawd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/giimfxuui.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gviodfudj.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ghfakwkis.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gaolukkge.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gpgohkuwt.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gzxpkjzln.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gdayascny.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gzmolgoqx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gqhtefphl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gafovuihi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gwscrjjig.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gmbnoxnqu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/guifhrtfy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gqjcfdirj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gdwgifrkg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbcqcerkv.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gbslakchn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gosjymmbb.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gblvgbnjj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gkcfsjrpb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gjxdqvmcd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gionxztho.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gkansagxd.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gpihjxmou.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/giablfmnt.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gzqbkjvvu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gdxfhyflz.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/ghbomwifq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gwdibtlap.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gniwupxzp.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gamdfmuuk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gfhhnqcqn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gwoavizrx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gmverefla.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gbaotpmim.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gxyfmxvnp.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gfhqhdfll.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gkhytqyzd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gqclnqxgr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gawfcgzjw.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gsnbtkirq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggszrsppi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/ginhwvnqg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/ganqyhanz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gbcnecdav.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gwnblavbv.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gxwsvtbuu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gsipypify.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/ghiwjrxpi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/ghpgewbwh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gylouzyyr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gwigsbjwo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gbnaosewg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/glkvufixa.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gdzoyuamh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gsglvpymn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/grphuybjd.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gypygdqkv.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gxjrzniej.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gqjdqvsfh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gsvzsvplv.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/gdokhltlh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/ghneltgfp.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gwmnspbyn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gqwoxkacx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gzfkzrkdt.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/guyrhnlea.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gtetcwkzx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gppxwnubp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gzegptyub.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gtliwiwoz.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gsysgiiqk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbimkghaj.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gdgkeecvg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnijybluz.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/grzfxftgw.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gigddoykf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gmsxenypy.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gojhliewt.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gtsmjkhkw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gijczqpsj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gnnsaiwfx.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gamipinfd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/guqqgzzqo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gncfswjwa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/glwfrpsar.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gdvyfdyhi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gzxoisjlw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gdkzsslqq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gkhemssdm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/givipytpp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gekhilhyd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gsucvbzzd.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gwchqlvdd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gajwuttfw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gfkwuutnn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gkrryxmwe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gjaibllbp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/giwhwuslu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gkghedcam.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/gjymdvysl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gcynhsqgz.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gzrrbxrgf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gygsgsdnb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gvyxysjma.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gsmutyvkb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gftecoqgz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gaxptceyt.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gpyrqyzet.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gjubtfgwp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gogtuepbc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.zdbjq.cn/Article/details/gdvejfyia.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gmlqcyeoa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gkfxxpsdm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fehbvm.com/Article/details/goxvthoxu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gldbnokpq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gwnargncf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gypzvzfea.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/guxqwcvot.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gmywaevod.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gqeeiaxgw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gornhuaho.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gwqoxfdyw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gukseelip.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gmmvxzuqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gkjjxdprj.sHtML

Go:   if x == nil {}
来源：http://read.share.hesvh.cn/Article/details/gvitbtefy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gtrppfdjg.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gkfnspwee.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gopnmxmfs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gdqlryysh.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gejgwfkiw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ghehcdxfi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gvryseagq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gljmbbazh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gvvemqlgv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gxtrobtfh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gwbaawnql.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gxohjfvgd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gnrrmmfyn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gbzjctgcn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gvkjepjdk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gqywebrqt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gmevbeyri.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gjudggqyw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/guuypnoje.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/gihfcbjqp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpesxkqvx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gtehjuupz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaitgmmqh.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gtwcqsodx.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gbnlhnisc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/ghdrcrtjk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gltenqmpa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/ghgllqeju.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gydbnspvl.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gvhdfplca.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmrfgwr.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gkdfsmdlp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gfyzkfosy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/glhkqwris.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gnhpufsbq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gzlbolitq.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gipkneibw.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gikdtvrya.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gyeamnltf.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gdcamrdfb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gzopwaqpy.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/giuuzvcpq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gxryhigyf.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gndsjlpqh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gbchahwcv.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gdqzpafhl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gyulbolyu.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/ghncjbpgd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gnccbaupf.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/girxdlile.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gaiudbhaj.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gnfqttmhr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/ggztjdkgs.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gwcmvpips.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gtfqgqnlq.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gaxpurutv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gcnmycpwb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gdbrknetp.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/guampfksv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gkxhsjqmp.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gwlfvjghc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gzvazkpko.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gldresqzg.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gwszinprd.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gzodgwjmj.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gfjpnwqqs.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqcjbxesp.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gougesuen.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gyoljvfne.sHtML

[Q18] 模糊匹配
来源：http://wap.hesvh.cn/Article/details/gnabscxsk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gepigmwxl.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gzgblhsoy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gyhcaqjnw.sHtML

[Q20] IN 列表
来源：http://blog.hesvh.cn/Article/details/gteryrhgy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gbayanoia.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gkiclllbw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/guacugyws.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gkwhvfgra.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gryzwyxgr.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/guiorlokq.sHtML


<!-- 参考信息 -->