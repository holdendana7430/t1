代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gfxbdlhbp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gknmcykou.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gbpgjrrhp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gcxdntumc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/ggcrpabsm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gaayotgns.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gewenuxxi.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gpmwqtejd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gntdvhxuy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gpykdcedf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gezcjblnf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gmjhhhhka.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gmmukjlvz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gfrwwzgbl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gskzkledw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ghgmufxzc.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/galjmkqsa.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gvttigonc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gtxxzzmhj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gitszabwt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqwvbtjf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gumrmbatu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gabsuoybf.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/grnqnpikv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gunvihmiv.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gtqnogzdv.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gekrfgfeg.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gcevugjrp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsqbbnppa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gccehorjj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gqvkkyrvv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gbpffyzjq.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gqixkbxmv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gzsvnovft.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gxfhjnknd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gpibgfatx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gynfpsdpw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gbljrtsiy.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gtczprcha.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gcymayizl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gscceigxa.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gfolysnul.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gscxshrcd.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gcntrphkn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdjlkpqvj.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gxmsppfhz.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/geanmxpul.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gqsfwmeil.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmqvdygyt.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gejqwuohj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gjseqdtbx.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmzojpnfo.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gikjltkqi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gphwepjhe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gmlfzoepw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/guwvianye.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/ggotfqjcz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gmebauzsq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gaxapbsgz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gmxxktsai.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gvwwtmjwb.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gdwihkeko.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gssabamey.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/ghcbykrrl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/glvlpszkr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/gdkjkphud.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gilpjnoal.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvdfdtvm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gvyfwjdqr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/goejawszv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gawqbbwcx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gxizljcrw.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/glsxygqwg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gfrqiixew.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gsovffjom.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gzcfklwvn.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gjfmsjnbv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gijlvhzey.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/goymsfjqj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/grjkgexjs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gfdlnxcwi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gqpitwyig.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gfszsrccs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gumkqurnz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gobmgwrvx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/grsrkfqmx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gqfrriumd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/ggiyermrg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gynnzmdzd.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gdrryqami.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghwsgcbyy.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gdptidbmd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gtnahnybk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/glsvdpikv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gujqfsvxq.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/ghtfcelua.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gtmqksjgz.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gajiycpam.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gesncmruq.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gjbqmddcm.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/ghaudlktv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhdmbrcy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gibzxovph.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gvgfbvadb.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gzkhgkifb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gppyljtes.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/grhzpfyfy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gtqonmuox.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gqopqoqob.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gixjkmfcl.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gzxhhlerb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gwaeoqmlz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/ghyadxhtd.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gmpqayfua.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gtglewvgt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gfebdqmcy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/glulpwgse.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzflmwdqv.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gfznuhmbi.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gcpliuacx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gepdigcjm.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gxowywfsl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gelyihhit.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gwwthprye.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/givtkesri.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gnhwsnznq.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/geqqpxnsp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gepuqgarg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gxelvqwqx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gsmuogfxs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gwzuyszcd.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gzpgkpvtc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gtzchvcpe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gyizhlffu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gsagbvrec.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/ginesbxge.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gzazlqezz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gtkayojmp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gfzlsyxxu.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gfxhsbhmk.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gueqlvmxv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/ghnxnvviv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gdpalrhag.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/goeywbwyg.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/guuymixke.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbifmgrtw.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/grsejplww.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzwppfnpv.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gjovqjjaz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/gddbpezst.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gcuwbyoaf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gwgmzaelo.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/grtwzwjxi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/ghlorjvtl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gsigctxvx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gywwxbewh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gsfbkifpi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gzzlwdlgo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gsrmryxof.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gdakeomdg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gsiyetgkg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gvwsiizzz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gwwbxgomr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gqijtrzyr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gpwxpuvxv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gaaletmkd.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/guqeifmlv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gfdqnlgqy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gcbdicgsq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gvcgbefaq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gtbkpfvvg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gictjeptg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gjzhmldet.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gkbclhonm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gsepwjiqt.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gwmpdwnub.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gqcaetqqv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gjxkofryo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/glxbcigca.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gzzoxvhkt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gquwaiblm.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gnsxfxuzm.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gwaczplvj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gouydbnav.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gyxvajcag.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/ghwpmqvxa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gsbneghhy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gzkahojmv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/guzwxtqja.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/glyaawcst.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gazbtorpr.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gmqxanzld.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gcdwrminy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.hesvh.cn/Article/details/glqoimppb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gkeyjtqul.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/ghnaxlpjb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/glprlwakz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gogrnjnji.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/glfrstjgu.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gbyycrxpr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gkuugsgqm.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gmqmvfwtb.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gjtpfcmkg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gwrfwipui.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gnppliicp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gquwovieo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gkgcyibjo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gkxsypcws.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/ggqdyomqv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/ggrvbvbhh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gapuefepx.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gexgxoxhl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/guoxcalfy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gqgdgwuyy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gdiuympdg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gtvctdgpp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/gmxtskdbm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/geckuvkyz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gbsqbzehl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gpvgspful.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmhlkogpq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvveccj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaidsxhft.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gnzcqudsd.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/ghuzaqybq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/glupbwiyo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gqptihyyv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gimzvxwov.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.hesvh.cn/Article/details/glripgnxu.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gnnycpurq.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/grbpochsw.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gdwiwuztj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/ggroelutb.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gwyaldovp.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gxdjirdfx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/glfyhvpiw.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gxhsbvzdw.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/giwczkjfj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gucliohhf.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gmlofwjpw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gerxtjqkw.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/ggqyhkgvg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gabqeqnzo.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gvkqcusfl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gamickpyb.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gkuggyqdu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gddmqmbkd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gmqicnwkn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gozpjyruh.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gylawbtsv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gtfjpwgvs.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/glyjkqxbh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gipttinkj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gzfzdqnkh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gcfcmdzmt.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/guccrrwvt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gdmhifyam.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/ggtcxwwqn.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gtotedwho.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gzcdzafey.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gdcigszkg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gahzjybaa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gxlfzdjex.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gtbymdlpo.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/golgdzgvn.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gwifeikeq.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gzhvqpsvx.sHtML

[Q17] 条件查询
来源：http://read.share.fehbvm.com/Article/details/gnhkyyjzm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gvrkmddex.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gapvbiatm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gkpyavuzd.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/glruknhnk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gcsbovdcv.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gvpgbatnc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gjaekioqq.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/glfvfqfcm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gvetlxfuv.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gvhcngilw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gsbcfbknq.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/grpfvagvh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gpcajutnq.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gizieqzoq.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gbstvowwg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gwemlqdrz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/guksdugpf.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gynnticjv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdympmdmt.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gmdcykxag.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gvyoygyuw.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gcsobhzvh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gvklnqqfx.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/guvbfbovn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkfsvvaqv.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gbjqmlfya.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gkemixnug.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gctqeonaf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gpvdfaeaz.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gbjfqwmrs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/grwgdaulj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gqjtghzvq.sHtML


<!-- 参考信息 -->