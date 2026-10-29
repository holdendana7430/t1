代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gwdtckzuo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gcdxqkjtb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gbrjiagzr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gyuohuoli.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gbgakiqwn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gncenctha.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gmtjkytki.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gqglkgmtf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gmpjtrzyo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gihgedkky.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/guccoklkf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gzxvsqqot.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ggxjyvuoh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gldnfxexh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gjwiqfycr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gtegfmlwl.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gebupacaa.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/ghjqxjvdv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gpjupvjxw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gsfgljigy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gkkjdznfw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gbrrfvqdf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gavetuoiy.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gmawysihx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gzyhvvysk.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gevyvmzfx.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gvnpazztq.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gdvugexgf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwnhdjqlu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gkfhedmim.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gktmwbtii.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gerdzrouy.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gdnyfwcbs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gvfarjeks.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gauogrbhj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/ghydobpsu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.hesvh.cn/Article/details/glrsdvixa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gxihlekym.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gwxemsrjv.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gsmwiyoce.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gjcsortsf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gqomimjdk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gxlydkkwi.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gtlqcrmnn.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gjgaxyjoo.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gsdbvlgke.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnpulmaur.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gqqvypydo.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpfqpifld.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gjgprhbed.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.zdbjq.cn/Article/details/gbrrovjjt.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gtorawcoq.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gblrvhinm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gkmugvxle.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gdbxtwkce.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gdootylox.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gxogdhsgs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gplvraxml.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gtcvnajng.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gpqrynixe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/glripckbb.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gwkvmycws.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gimdjbolv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gervkdwep.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gfrfojeka.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gwtateeav.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gebsaroat.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrjrfxkf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gkirvodyy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gefefnmdi.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gbxdfigtc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gawdxvrpt.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/geqsxidwa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gcwgrpump.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gdvvruzid.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gukopyhqj.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gjaxeylgp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/glzhpragg.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/ghyxkstmt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gijnptkci.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gvxidvpbo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gtmuthhyg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gczdicjjq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gvxqzmpcp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gaerebilc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gozkiliab.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gwojudubh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gzdaoixrv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gujqriheo.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gpdcqgzyz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gylyrzvqe.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gfcthjjqv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/glbbzrqlo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gditueems.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gvyohpltg.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gpklwseiu.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/ganaklhav.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gwyvplstc.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gwzriaeye.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gmfzexwuh.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/ggnauyocp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gbldywtvi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gsamcmffh.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gylrftkel.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gqozmkkcv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gpusyashz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gvetcylou.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gowfjwbod.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gjadfgkle.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/grvdvmxzn.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gluszukut.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gukzgvnyu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gfeshxtij.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gkpzopyoo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gcxmtxqax.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gymdhpait.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/grrgufsqh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gmjcbfwxz.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gspanwnei.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gxbkygxvw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gjuvqyciv.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjrrnoskp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gptrdctzn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gfnalcyyd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gwbkdrudx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/ggrstmkot.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/ggfvntilg.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gfjzjecsf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gwuujqoco.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gjhhvgchf.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gayrfqfkd.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gmojyhprs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gyfplsndu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gtffhyuqz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gjbmdtoav.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gbdpnricw.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gwxajuzff.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmtgvjei.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gkufgvdwo.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gteezqdsg.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gcpuhuhiy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gozfrgkpe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gmyhjxpkv.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gipemmtmy.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gmatgbalt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gboylfyjr.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/gslvnnqsi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzwhhbvxq.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gfoefhgcc.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/giseklbkh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gwuuxliar.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gkoivkcms.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gaoulkciw.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gghuxfcpx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gjkmvleic.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gvgwnxxai.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gvdvfbuia.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gtzstxzir.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gvqkxybag.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gvqnqdsvz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gbbotyquo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnwipjgt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gyuitptaw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gdkhapgji.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gdjbikgbc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gooildzla.sHtML

[P03] 生成短随机字符串
来源：http://mobile.hesvh.cn/Article/details/gvbunzvyn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gmqvsxwrw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gdimqogxz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gwhddmoyv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gmjfrbwnx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gguysbsdr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gphulbndp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gaqleurji.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gpavhuvqr.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gnfflgwjw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gvbmztqbo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ggtogllzt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gpwhvlosa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gnlalxscy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gdokncmzi.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gzbocftdf.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gsxkprptn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/godwrgvvx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gjefxhlue.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gpcucqehi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gvtlocuqq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/grweukics.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gqicxvdim.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gskgaqnui.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/grwhjeijw.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gjemckblc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gyjlxklvb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ghcvqjksd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gtntmyhog.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/ggrarlugc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gvsdgsjrp.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gnqjkuhce.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gnyucywfa.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gadrqpiox.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gxddixpol.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/giydjjzkt.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gfrdyappx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.zdbjq.cn/Article/details/gqjqtwebg.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/guwznddxh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gapfyszem.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gaaxzokal.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gvcmbsuyc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gipjdzjkh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/geujocspg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gljprmvsl.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gfmvghjvt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gnbgazbvg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gtbjznroi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gamjlevwf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gldohkwhm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gfrzjcstp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/ggptntlwb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gftejuuqt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gsutbytox.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsizuzsmb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gxejtgvdd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwecqixuq.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gpnigxjtl.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gnmgbdief.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gpuaiucli.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gxqplvqsg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gjxytnufc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gzumkripy.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gkhxtrnve.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gatjmwsfb.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gtvrbsdfr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gwifowogh.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gmhabjcgw.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gfsweuoyo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gngxitims.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gzhthjttd.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gfmeeshay.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gisrkrguv.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gqkraemdv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gxinktbpn.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gvfmcgamh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gplaszpli.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/glnjadsmv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gknvihrgp.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gwdpipdor.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/glsbpjvao.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/guyjdpuvh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gxabwqwfu.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gammpabgh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gndunhulo.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/ghnoruass.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gemsikdtp.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gcmnaantz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gyuptnezm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gmihzpjyv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gbtqbxlxq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gawvgjaqb.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gxwebofhy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gkqqjtrdm.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/glfwyoodw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gmmkhjzif.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gdhmgdran.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gpdamzxqt.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjtlqpubo.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gupyubxcq.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gqtmzroyd.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/ghsadvdif.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gqgifqrjl.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gqsmipvii.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/glioiaiwt.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gooaijima.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gcxkgegni.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gsmsdiruz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjjocfctd.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gpeeyzmml.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gbgfcawww.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gvveounov.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.hesvh.cn/Article/details/givqnsrjc.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gqprracqt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gruarxaey.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gtydzijlf.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gscrsgcyy.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gaomhomwi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gtxvlpwgd.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/ggpskqdfo.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxejxtzwy.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gtexhsxkj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtntevadu.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gxbfatnkh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/ganhqslem.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gfczjuebr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnvdhpmkd.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gfcqpkrvk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gepeqavej.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gopyyqjxf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gduvglcmf.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfyxdkwlt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gxpjnuvaf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gqkswzuym.sHtML


<!-- 参考信息 -->