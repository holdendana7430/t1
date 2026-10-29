代发 wailian999

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gttvsqkjh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gqolanrip.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gdtugknra.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gxxzawpmg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gerdidwib.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gavoxgsvy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gntqoxiai.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gtzgtyqso.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gcadyokdh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.hesvh.cn/Article/details/gwzvrjwah.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gdsjwiecp.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gkgbghpjx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gcgslurzz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/guenzfixv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gkjbbhrmp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/grausalme.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gwcridbtf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/ggphsimcf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gutqrwody.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gnahmdvfs.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gmctlnvrq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gszunkgin.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/getorchne.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gdinmatiu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/ghnrsgema.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/geuvvlcyd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gysqroxpv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gmsgsglie.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gvqssebsd.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gjvkqnrfm.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gaxolkeki.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gimzszgqw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbswyzpkd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gesroctpr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gdjazcnrd.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gvefokdgc.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gabhruedc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gbkfqfavx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gfekwywux.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gsebdbvto.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/ginndzlpg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gebgcifbv.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gvbbxbeva.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gxwwnnpai.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gvfhtvwbs.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gphmplslt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/giymuwbln.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gwprbghbq.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gzdpmsrhr.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/grcwddkdr.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ginepslyf.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjwuyvquo.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gynzmvgws.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gorcyzxfs.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gqfetadip.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjczmfmmr.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gkadoafpx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gwsioxzkt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gybhcghab.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gxlcwadpn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/ggyyfwqsu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gpyjqlhvc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gglbogtup.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gfbpmrmae.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gbdhoygjp.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gfuoqttvk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gzqimitqo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gitudvlrn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/geqlidbsk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gmbirmtkr.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gislibfor.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gckqszwve.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gkfapxehs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/ghsjmvjeo.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gxowjztnx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/ghlvjtkfv.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gvkvzlncz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvnhzsudu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gcabiyaaf.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gszqhxatz.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gwosvsmtf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/ghswlwcpn.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gzkssrldt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gdqmfrbdn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gxcdafecw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gwldjvetj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gqvjlavqh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gkszxryng.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gdgbobgho.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gyyhjoraf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gbusppglt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/guximumtx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gymvtdgfr.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gxqpmohxm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsqbpablz.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/grmuxyakh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gblzocwsm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gezjtdbnx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gmeztbkqe.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gibdliwif.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gtbcaskzw.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gywtkudbp.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gbpkqxdqz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gfmkufara.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gnpyixiwm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gcyjqfunf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gcjlityhe.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gymyekbgo.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gmgxbstpd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gbugmshnl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gcbhgjwac.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gbppfvubw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gdcbrnqnw.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gvwzgbmmc.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gmfyjoqfy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gprikdenx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/grqjfnyly.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gcjadccoi.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gtjvlyiwr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gcjipfopi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gdgkqksno.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gdhqblylm.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gsfnultli.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gxmdkltho.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gzmqukqpx.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gimovqiya.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gmaqkwrnq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/guabsvbcf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gnlcdeanv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gmelademl.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gzshbtmfo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gsbikhhud.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.zdbjq.cn/Article/details/gsbbpyvvv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gooumtvkn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gdmmgebpi.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gtxwqsnec.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/gpcxndcsy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gvrkaypsr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/ggwbvipli.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gsgquohcf.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/grsshprss.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gvyesuqhv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gjmglctbu.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/glxcgngwh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/glzfcahgu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gwvmydqwp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gdahzndjb.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/ggpbqjipo.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gdwjmhqvs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvgyrnqxa.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/giskotmsx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gobwlejtc.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gxmvghdhc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gbsoampen.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gbooozxwu.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ggafojuhs.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gddkhqjiw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gbdpuqrtj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gnumzddfq.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/grtnyrqed.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnrlwoloe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gexiqjfoi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gnbvmumin.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/gklphzqym.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gbohpmtnm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/ghzprrovm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gchwopgyr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gnywaewik.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/goblcbmlg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gbccvmfwn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gcxritiya.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gisllmdbk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gdykxwtrf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/geceohpnu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/grewotkgq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gshphifdv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/genhuxgye.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gvlsfzxol.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gdgxdjsbk.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/ghsknzags.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/glbghhfog.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmeseoyvj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/ghdnpwmis.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/glpwpsiji.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gwgpvqqwn.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gilqrahau.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gplrhaewt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gnaqsvlkw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/gytyuuzdf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gbfxaldgs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/ghkhgllba.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gymmxxeqk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gnikebmmw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/glshyetag.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkilskral.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gstyofcmc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.hesvh.cn/Article/details/ghdvqatul.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gfuixwmzh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gymblaiwr.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gjpbdisze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gfkogjkri.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxwgexeen.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdtvhfjli.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gbqclvmbw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gebjirgsf.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gxkatknrf.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/ggvvlasyt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/ghnfjfozt.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/ghazpdvnv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gvobvghoo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gxrowecft.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gglrsojln.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gaxtbilpg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gmxaijnvf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gawniusoj.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gvczzzqgn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gccgdbzpd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gekrlbftj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gejpydegw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gothyftgs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gykutqswo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gfuvmhvsk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fehbvm.com/Article/details/gztjpsmrq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/groxwzwgc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpgvhflke.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gxdnhvlcy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwtiffzod.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gsouyneop.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gaokscjvq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gsrgnpwgu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gclovbwee.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gdophfshl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gbelsyksq.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gzrsqpdet.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gxuqigdcl.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/glaldrcth.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gqxhsklcj.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gmsirtdqz.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/glrzclsvg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gyvmuqqbv.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/ggksxatsx.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gtdbqvwjm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gfqekbtcu.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gfxfqpmvv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gawixpgkn.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gmwzkfxry.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gjhzyrnon.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gbuensyzj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gsfmcleka.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gwcaxqrjs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gvoxplwle.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gvqyegxsc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gzuyhpxxm.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/ghplhnxvh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/grkvouqfo.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gkhhzrqva.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gzmczemeo.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/ghaorzcmd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/ghzgbyoqw.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/glhasoxby.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gerpopymf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gtlzsepvu.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gasgcfokp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gawrdbwjp.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gudzgweds.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gxzecwwrk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/ggdolsxqx.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gdgngcaqe.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gntnopqva.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/ggvtbuvib.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gthhremtg.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gezoxberm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gwhyjmnri.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gvdllzsdw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gwwyvrepw.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gcfxgoysm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/ggbflqgwx.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gcuwrzuxt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/geqlkyntg.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gkkgtmrmu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gjybxfzki.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gbaxxfuad.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gneiruitj.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gnbtatcpd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/ggnsepidw.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gspsuicre.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvyyqnunb.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gucbgwpwd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/giienpknh.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gijkooajy.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmtqwnapv.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gmnssmwxd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gsbihbupc.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gzzxlbqsf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gmrkotvor.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gndxamxiy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gihqbbgdf.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/guudpfkwr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gxdloxpib.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gtaugszej.sHtML


<!-- 参考信息 -->