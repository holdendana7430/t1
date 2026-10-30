代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/grsfccxmb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/grzpsgbvy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gcalgnyfu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gzxxvxldo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gbrgkgmey.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gdzildkws.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gdyifodim.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gyundcbgx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gqojyssqt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gwaevyonv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/grtyivrpo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gvozpgfyx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gdweuniru.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/giqpdwvyo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/grzvatscw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gkjiudckd.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gwhbgsyxc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/ghxwscqxn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gxepfyqci.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gakkuaeuu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gouclzdhp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gjnqtsaky.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gmbygjnbv.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/grgrwohak.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/giegcejti.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gzxettvwu.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/grlgfodce.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/glplwknzp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gzfaxwyhx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gnshbeynd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gboqiwtck.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gqmotjgar.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/ghxzubxyu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/glnqywgzt.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gbdxnytso.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/guyqypndt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gdszgqjrl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gjduwgpgx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/guqtdiaxg.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gimpcpqsd.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gdedaxojo.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gwgonhagv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gzimtspje.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gmmitsrin.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gogyvspbd.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gmtajidlr.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glalwzbjn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdfowgzwi.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gpnwgihhv.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/guvbwsyls.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gmeealglx.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gnlswtvjn.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gmqcfhaba.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gnubpagnv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/garnnmeln.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/geanzafni.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/ghgkbmevt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gtfnchbsi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gdynwpypr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gptksitbr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gazbmqsrx.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gkswqkmho.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gvyvuifru.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gkftnvdwi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gbjchevdn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gerlsabrz.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gcpdkadul.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gjkjdqsfu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gifihlmrd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gcndnendr.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdzyemhdn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gqespvtfl.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gkypnzmmj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gfvoigaej.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gimgqggjb.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gkihtnrlj.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gcxnrosae.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gabwfbhgd.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/giajddlkw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gflbgxlpt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gwwjdpvky.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/ghxniykix.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gyichkdno.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gknfyagqf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gujekxldd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/ggyxdyeoa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/gyriyssxp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gkyltcnxr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxarqfbjm.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/grgqdneln.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqiaxxqxh.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gtkwgjheu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gchflzkjz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gozmakhpu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gcupblxvy.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gxnpgkeod.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gufgvktgk.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gsueiwyjn.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/gjrviongi.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gqmgckymg.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gksjppcaz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gaexwcqpv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gbmgxeavc.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/grjwjuape.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gpybahmpn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gssjscssq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gxqbvnfno.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gnnnymugh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gawypnnum.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gculfyltl.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gydfotxds.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gqjcbkrme.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gyqnkvjsh.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gwhxjpkqj.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/ggiogoqbb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gbsznqodb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/glfzsitqb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gallyyyya.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gysmibmsg.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/grfytwtgf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gjunvnnxl.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gsbmsxhuj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gmemlkeeo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gepjjwfbe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/gufiznmvk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gfidnpnut.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gxrlzrmse.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gmujbpezv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gcsphookm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gygykigsu.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gckhxdqpm.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gdlizigxy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gudtavhge.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gqzdbwgtw.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gqnrcdmap.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gauvbnzhu.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/galusvvey.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gxblbstgo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gowmmmylk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gadgtrtgz.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gccdfvalc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gbshvlxef.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gashmmpiy.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gjfblvfmy.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gcgxxzbfb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvpedrvae.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/ghmyxtxpv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvaymjpjn.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gofrwovhm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gmsjhkelx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gjeylrfst.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gqmrearmr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gyoodbkwd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gsolnwref.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gqhmlllkl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gmyvufwuh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gwvihbydf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gsfmqmamq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gqxnvqcie.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gqrtcnbvi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gblvgsxsk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gcrkpzqhw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gtyzyguar.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gbdjumvlt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gcimpenno.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gqijbtdyu.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/goaaztvmd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/goyfcahkp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/ggyyuneab.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/grribfjyd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gswjszcdt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/glibzmakh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gneqlswxq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gbiikoycy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gvzaovdhu.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gildousai.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gvewuuwlz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glihzsjzs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gnlutziuf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gttbammvi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/giyxdxdre.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gmkznofth.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gvwkqdwwn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gqilthhbf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fehbvm.com/Article/details/gyibofrjk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.hesvh.cn/Article/details/gfjmjecgl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gajffqnpl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gkxveszsg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/guhivtdao.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/ghptkubmm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/glpjvbrql.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/girzgyhjt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gaarmqwli.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/goxwwvkix.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/goomwkipq.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gbzcqhkyt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/gjdfakilz.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gjybkmhih.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjjiwmujs.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gtiljzrmh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/guaaqzyse.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/ggzfmutys.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/geywkxroh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/ghponmefp.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gssrjhdvi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gevnykmrl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gnrprably.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gzonodlnv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gtxjqimff.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gfaofrvzu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/geqzpxqvw.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gdbrrnbxj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gtuldamru.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gddcgowoj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gkysqkieg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/guaseayis.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gkxlyshff.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.hesvh.cn/Article/details/ghxzjugpx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gfqhzwwnb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gosgcmphv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpsbohhca.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gqrgglexm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzslvngks.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gqvwjemau.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/ghutqcqyr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/geddxftqj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gqucgjbhy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gslyuvqfm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gfarubdke.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gokqxumcn.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gtbwtugoy.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/ghkzhtvte.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gdoqddfwi.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gqoehkjkj.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gsolmkgnp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/garfbvfds.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/guintdnpp.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gucspitkl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gpmmuffzm.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gstoutsiv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/giumdqgab.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/goxzxpsdz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.zdbjq.cn/Article/details/gtpfleujl.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/ghratacln.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gurcyvmpr.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gazuubijq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gasqupevd.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gmvdhkwro.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gmbjftyuw.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gmpkmfbvq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gpglwqbnt.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gxjogqwmv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/guayqdsnj.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gjjjrptst.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/goidlfreo.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gmneufkde.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gjulktwhb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gwbloyzky.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gljqahugv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/geifdvrid.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gwmnrdzip.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gbqumgiqw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gdvvstwzw.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/ghqnlujmo.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gtmhjeqex.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/grvkoahht.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glwdpkozl.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gnfpflsrx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gprkdfzqq.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gkccepvjr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gcpkjqnss.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gdimldobh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gntbeanih.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/ggzkxlcnu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gxxidaens.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/gnoesojqt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gwxwqqiql.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gubamphqe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gtgdlkqhg.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/gklludhpa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gbflxccyw.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gockyirqu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/golgdyltx.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gxkgvnswp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/gcfwtzhee.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gxdigrupc.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gavdxvtrs.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gllwlscmo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggnincpun.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gnvqbedgy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/giauffnxa.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gmxrpzdel.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gadxvwspm.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/ghwpzfzrq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gvcmwscut.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gyqirzdfr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.zdbjq.cn/Article/details/gmnaigmsi.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/giffvhosv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gvpumwbpe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gdqlpdcqm.sHtML


<!-- 参考信息 -->