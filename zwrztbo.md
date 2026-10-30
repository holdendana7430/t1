代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/giaugefpi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gcmjexudm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gpcvclmmr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpimpbawx.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gveboiwiw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gezsotzyh.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gvbbiceqb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gmwhugald.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gschaeuss.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gshvvequv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gvhkcirnr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gqzakknvm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gyqjyodcm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/geebfiwkb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gembqdikj.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/grqdlrtqc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gwtqraiuw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gyokwirbg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gqaghwdim.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gxxmeugax.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gixdpansv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gsksjjjpz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/grhvypueg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gfqfwggjx.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gzsmiwfpu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gydblbzrb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gdhwgvmjm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gpnnrnqnp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gjbfywlgp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gnegjrufd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gmkvzmjmk.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gmhkahkca.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/guautxhms.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/guqopnywd.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gxbbubcmp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gzlbjdyvt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gzpdwvgfq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gisfqabwq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gnenmwxnb.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/grongjghi.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gclrpqfmi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gxrhswinj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gkoroibai.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gkwljufbi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gxfcrunnc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gqavlbssv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gmgjccyst.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/glapuupdj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gemwbvowc.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gxczpnlzb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/giowiavon.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/glcxnaabw.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gydlqscun.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gcjyxynzc.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gipfvsauc.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gobpgfsmg.sHtML

Java: // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtzarurvj.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gkfouyvtq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gywqeqgbx.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggfdhretq.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gvvnzuqmq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/gasksedeq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.hesvh.cn/Article/details/guiozmihn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gqvhnisnl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gouqgmesy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gqjjynifj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gvufcjiay.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/ghvxjzpwe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gypgagjhn.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gianohfrw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gyolopwzx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gungjgdze.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gpwkibqhh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gafoyhedx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gyxfdrzja.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gegvahsuq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gvxwkyyds.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gvljlcljt.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gufjsewvn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/ghylwvzzt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gitkgjmnp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/guywmlntm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gmvykswen.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/giyuiehub.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gubjmadgr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gukniwyzp.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ghmrzdakj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gvdodnujd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gkhptonls.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gzoblgkwu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gwgpzcajf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/glhffujmu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gnibgmrzn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gnhgcchki.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/gqugbupeq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/guxqcqctx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvawngqfo.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gobrvspet.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdjnerjxy.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gilveiyyi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gtljxzmra.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gfuvxgzyq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.fehbvm.com/Article/details/gpouyobzs.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gmwfrivky.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gfcxwmpwi.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gehmowmia.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gdjzavxjm.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gndnbeffp.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/ginnvbvxg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gvmkqyukk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gnkbumvvm.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gepgsbhly.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gjounfgzt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gowwtnhqy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gjksktrge.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gytbxtugd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gxiemkypq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gmttmoseo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/giuaswtgp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gqorxwdno.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/goretaalj.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gpukbzlpk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gotsjzdxj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gdgcmvxmt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gawmxeofi.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/giaetoesn.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gznqyfjzf.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gkkamkfin.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gyxgckpiu.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghyvgjivs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gljnvzhuv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gjjprpfes.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/glnolajcr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gfhlqdawp.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gbmmxeygh.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gyjasgztx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gxktjlxcv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gyehlljea.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/guodjtxhi.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ggyymctar.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gugfmwuaz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gntiovsox.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gapvnyrvx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gdgyitrmz.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gchvblokx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gveypgkcl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gjvixbnjr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gvxeqvhsq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gbalkvwxr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gsklorsin.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gknpyqxqy.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gyyqdvxmp.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/gwedxyjoh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyecasijh.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gbsaqnxej.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gamcgkkrj.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gjpazpkpv.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gfpebntbt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gvtdtjkrp.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/glmqctxts.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gefylruul.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gfaugswwa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gkdxdmnjl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gpnztesaf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gworgnngh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gywvssjvj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gixkpsafd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gnbnnntfi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gtgmcqlrg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gcbkwovfj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gpoemwlmy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gkagdxcng.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gnowhpdrd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gnsenttfg.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/glfkerorr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gxhmsmqkj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gqirvadrb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/glznqiwrf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gayducdze.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gceyegsdf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gyipbfzyz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gxoubmboq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gymgcgpcx.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gvbjmlnap.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/guwlldshs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ggmssqldn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gcshahvaw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gtbekhzfo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gitvtqhhs.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gsiryekas.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gzjgvilzq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gxjshfems.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gnhajuftl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gdukdpgcl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gckodkifi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gemhwbxnf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gxjawffbo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/goqfbjzog.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gpuymbuzb.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/garcgjyzk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gmylfbdjx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gcgcsjllw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gdcvspais.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gwudmkfda.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/ggejfhdnk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjxahfecu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gavrytjjs.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gdpofvfek.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gkbhkqyjw.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gibikwmrb.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gflocwrsu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/grykvpyya.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gjdflxvrq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gllweforw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gokkauibv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/ggwmpgrig.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gjsckwcsz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gmajsmcge.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/ggteqgrlv.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gjaevhsus.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gbibpvtww.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/gtgciwhmj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gnctkxvdf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfjrnyup.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gofycelot.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gybwgsoar.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gxqjbfnsv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gtegxaflo.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxnphwtpu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gnckgcahw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbobydvdo.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gyhshlxfb.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/goybaqdxq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gzauxapcc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gkkdhsfpu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.fehbvm.com/Article/details/gbgsoselo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gktwtdaxu.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gasvwvpwn.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/giievvsjm.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gjxfrwpbd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gcmkhbqhx.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/glsdkrhws.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gwucrodxc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/goeqoyzsr.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gqtdnozgw.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gaymwskvi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gvdyqvncu.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/goutzpheb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gnxueloto.sHtML

[Q05] 重命名列
来源：http://blog.zdbjq.cn/Article/details/gicvyxiwi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gpzrkjrle.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gdlegdoqg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gckkquasi.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gaqfdnoar.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gxihnvilf.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gcojdvexz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gyhnyrirn.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gesarivhx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/genckralr.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gilgxqwim.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gclxehmmq.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gunialiwn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gicacthkm.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gglruxoxh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gyzpnqabk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.zdbjq.cn/Article/details/gbeobvdcf.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gefdohlds.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gysxlvgtm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gnwlcbmeq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/golbozert.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gperyihnc.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gqxfjgipm.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtejhlvbu.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gqnwhcgnu.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbxwzghuc.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gbdsychfb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gvxcpbdso.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/ghihpgyyl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gqbmvlfyy.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gbozauuhi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gjjjutcug.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/ghfmmfgmp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gbzltlfqb.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gjufiordg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmqecelnr.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gjnvevzue.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gooikoknk.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gknmupoyu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gtvyfpsmu.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/gudiablbv.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gytandsyv.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/grrdgvgvr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gxygqbonp.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/glplukmij.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjvmdteld.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gcinpwguc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/ghioiaugi.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gioxmcngh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gobbgauiq.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gdlodhvlq.sHtML


<!-- 参考信息 -->