代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gbsxdfwdc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gxxjvjupm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gkdfwgron.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gowfwvxdj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/grekxwsod.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gtbufeyus.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gjyxsntjv.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/grrejjbia.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gdfbefvjg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvvjixfu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gpfhpysla.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gkupafbyn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gtgwvadvc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gcmoxkwpi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/goqtmgdvj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gakcwkxup.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/guxodqzyz.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gtuboujob.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gjbfjmkkw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gmtaofals.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsfgmkku.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gardyrosn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gswvjqqbc.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/ghadocfer.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gqlcjxlbs.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gsnxgjfbw.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gliluqabi.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gotyodxte.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/goorafnwb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gxmkuckxp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gqoncjaob.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gegjlnuag.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gbskxmudf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gbgiecjfe.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gxpzlpybj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gssywdjjp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/ghemcbmjw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gqboiqmcn.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gvqkdgymu.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gppqqzarv.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gclplvxuf.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gibbqujwj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gvckfftux.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gcjxdltdh.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gtlfpfllo.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gqxdpowxg.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbsfxpuuq.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/ghwpfkwiu.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gmhuckdpx.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gbamjpggs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/grtyboxie.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/ggpywwhoh.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gwkqhhegb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gzcfzctbx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gqyshurnm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/grkqefbrx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/giergivru.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fehbvm.com/Article/details/gzexvrfhj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gnsyfqbfo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/giomwlirr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gytqskara.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/ghgihezpq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gqvtnjtkm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gjoxfnudi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gifcyokzt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gkyblwjoh.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gopazzaxp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gvjhbzhex.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gppqkwuyf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gpairqikz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gspbpclub.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gipyuyvcw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gzkllgppz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/ghbartfbk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gdywanhjt.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqsfpxanz.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gojgnocqo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/guznauhoa.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gndzinnfs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gfrwmybbe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/guklaqojk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gbpptxewx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gprmulkhs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gtlcnfyek.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gjwgvmfzb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gnkbntyam.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gjxtpedsw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/grkzrqkpa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghbjvtyjj.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/glbxowwxi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxauqwgcm.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/ghaxaidye.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/ghneokjpg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gzyrvymqf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gwvyamofh.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gatyufixc.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gzqjvhbkz.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gbtnzqmae.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gbxvmgiwl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gjyrypkpq.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gqgeufqbp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gnpzwypid.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gpuqnimml.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gncdqdrtp.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gdcavuxky.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gxqtfvmoj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/gkihuindd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gzesxyacp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gicebqtat.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gyednlica.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gxotnvnwo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gicitaviu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/ghhiepycj.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gnynvjdfq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gbeldgrgi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gfsvygznz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gwnrswxhh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/giaoixiba.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gcznwwzir.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/glkvfhgtc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gqeisdhtc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwokbpo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fehbvm.com/Article/details/gcgkigoel.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gvwqfgnux.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gsgydsnlt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gbmxjoovs.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/ggtlocbdt.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gzlxbtqkl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ggfkmisuv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gwazdnoch.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/ghmwqwcpt.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gkcoaksmz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gnxaepmng.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gyvdogwvg.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gidqqjwtl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gawpftatw.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gfcxgpugs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gcpjdxcwz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/glkazpzov.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gewwyffhb.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gkiugnocc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gmqdjyygc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/gzjsnbpuv.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gmxytyrao.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gumsfelrk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gexgvhwca.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gkxvusxun.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwfwseqar.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gyyodcujo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gfnwkzuay.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gzzpcpgbn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gmovjdkrh.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/ggdnoyjhh.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gsrkbqzox.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gsxczrtyl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gpywkwjgi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gylnmkicp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gzbdhjyko.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gnqbroxzy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/glnmczgvg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gksuojwzz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gvzccdetw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gvgqdgrlo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/garvpcrzv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gqhybqwyy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gpexiqjre.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gznfohprb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gsuomllmp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gumhacdxn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gjvmrgxmt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gyyhujgos.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/glmwdhtsc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gbljaxyao.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gjmvfzbif.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gjhkkycai.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gfybskfiz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gbojpxptw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/ghvrwponz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gawelazhj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gxvpdglfa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gxmajpjwh.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gjtrwhiks.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gopdeeklx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gsaxzmurr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/godepdgos.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gxakowgvk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/grtuxctsc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/ghnvmaani.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/glcgezjjt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gkibyijqh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfqgsmazt.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gpntrxuxr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gejfvovys.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/glxfkeook.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gcosysqam.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gqwpyejvp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gzzkofqss.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gwbzvgwvx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gwpsuvmfl.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/glctkezld.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/ghzneyvlg.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gxnnxbgac.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gxtunbbku.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gvrufmecn.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/garqatxjr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gbuhuwmzm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/glpobycbp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gobogzvqu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fehbvm.com/Article/details/gkwbzbzgd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gwrnkegdn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gpuxrisws.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/gehbiuaqv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/ggljvgchb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gdgtlfbqm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gmjovvopt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gfakwbhcd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gwmhziqao.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gvnqhlpux.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gsepsruzc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/ghqjqesnx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gztvgheox.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gekeuvvsf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjwqvvkwn.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gauuuwyom.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gseapbbnj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/ggkkkddyo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/geozdsssk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gfjtmsdud.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gqptlnuth.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gtizjmbvq.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gcjicqamy.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gzvccxjed.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gmfxeawfw.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gfpxxbcwx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gopxfdbpo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/grngxvpqy.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gygtfkfhu.sHtML

[Q03] 增加列
来源：http://www.blog.zdbjq.cn/Article/details/gqiturcjv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.zdbjq.cn/Article/details/gwgpowtbu.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvrzncute.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gdtgfqmdc.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gvjymzqfl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gncqdqzxc.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gbbulvfuk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gjpvhcntv.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gpeeswwvw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/giwnzuxrc.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gxkdsltgx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gbldsbwbl.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gowhlntch.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gydjamfpx.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/garajwxoc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gffciewse.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gmncqyzhx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/ggyemukfu.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gegobfnlw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gfpwstdmp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gtxoukcak.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.zdbjq.cn/Article/details/gkjjjbbpv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gwqotyynt.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gdkhajgap.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gmxoucoam.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gsclkqjay.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gpjczyhmx.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gcssgsoiv.sHtML

[Q16] 查询指定列
来源：http://wap.fehbvm.com/Article/details/gjadzezdx.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghuhdeiwz.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gcbbojwoz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/ghmvfaxdl.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gluyaoxff.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gyexenevs.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gdvtwdsgs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gmizgvjxz.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gkeevvnyx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gmcnlbwgh.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gdedtcslu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gdunhftxl.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/ggaalraku.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gquiiyvsa.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/ggkmnbgop.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/gfshtopuf.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/grrsbcmrb.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxswppdlo.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/ghawctdhr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gtgaviapo.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gsaqeordf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwwvribms.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/ghcburwpc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjfofdbud.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gbapfevvc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ggbgriuco.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gtsvvalkp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/giphjvaim.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gqpxicwsd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gmreocaef.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghzvengxo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/giqukcdmo.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gccrigvqk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/ghkbdlrtz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/getpszkak.sHtML


<!-- 参考信息 -->