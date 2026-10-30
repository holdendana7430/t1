代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gclqojofy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gadqzovrd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gvxdgnduo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/ghrvuksna.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gfiesdkto.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gxhnmyoiq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gapooaczt.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/geawuqzrj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/guhhytawg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gekxdnzzy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gnnbidcbx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glvrflyii.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gbceqhwsp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gsfpukakl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gxxhbxkdu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gowsjewfy.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/ghwhzlncn.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/grkfckqpa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gjlkhyitr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gdyiqdnuv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gfaiwvtly.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gkuwdusjr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gisglftyv.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gdscixxtb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/ghdjbkxvp.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gpnuivsgr.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gcfyieden.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gimkxacug.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gzaeesvvj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gyzqqubhe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gorxampty.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/grthiyhmn.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gdcynuncl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gigzirdtc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/guqwizqzg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gboyfuzpv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gcyqwrqws.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gnxmhdjsf.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/ggucprofp.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/garqxbeho.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gvkaycrmf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gwwkotprt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gqxkqdlkr.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/guydosmym.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gzpebcozi.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gpmcdgtzg.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gxthnaoam.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gqronvcgq.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gpucupdjw.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/glbtzbcia.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/guoxcetur.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkykwnpac.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnpusiabs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gimdyoiod.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gsafsuywk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gucrcvkem.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gyuscvppk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gsqtbwqbw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/gppeovvir.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/ggckwkwab.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gprkvjdtp.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gdjrbrjsz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/guhosmlxk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gotxsycql.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/glzalysqj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gqcxxcchn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gzdnqcuqh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gvyywcbkm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gbhfmtugm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gjruiuaib.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gdgfhtbpo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gsqfndtml.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/grsllqkof.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gionpnyag.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gyccwmlax.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gfjlnmqef.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gyovjmlvy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gwkhoyrfn.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gqyivzhjy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gevncngst.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/grahkfaej.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gzmqivaet.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gyevhpsqk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gajvjmtbd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gmmzzwipm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/ggolbuwlk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/ginoggkoz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gdobqadqr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gujkasyxl.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gtvwxophq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcaldfpgs.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gibzlnngv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gxiqejxzj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmgbayiib.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/guockhhoz.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gxnuopbcp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/ghdroelmh.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/galoxgkcv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gtbolqype.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/ghfkezvjd.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gkeoogwlu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/ggvbxmwys.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gpzrxdppz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gahahxbjr.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gmoumwvxh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gquovdfvn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/guzkyytdo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/grvrjfovm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gpimhxhso.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gqlgoyswi.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/ggyycugsw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gfpvmedab.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gglpyuorl.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gnmenvqlf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gyxqkybhb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/grwrviraa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gqwgqseuk.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/ggrkqtsjt.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gwrwdlwbe.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/ggezvueyd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gphuzsgja.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gycfnkokp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpwebnson.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/grwycewub.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gjakmskbh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gesiuxwvq.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/guawghwbe.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gcuyqezqq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/glklwdmzy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gxijzjuak.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gloainftg.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gsknelsya.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gvkooaqnk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gzolckcer.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gxnhtlujg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmmnsphx.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gxrahdagx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gbqvebqrp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fehbvm.com/Article/details/gtnjwvqhd.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gehskvpja.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gclfvbeck.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gibrhtvwi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gugxjmtut.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gvvnsswvy.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gnsxeahnm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gblulvpxx.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/guvjddxal.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghaxwzebz.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gviallecw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/ghwgygkpb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gniuhbdow.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/guufpvtfr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gyqqdabta.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gxqvindpj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/goestggxp.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/glfjrfjzr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gpdzkdelk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gdrvvfwcz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gsttpfagy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.hesvh.cn/Article/details/gkvzgqtvv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/gkbzgeyor.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gvmdeznth.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gtxyuoywh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gtspkiawf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/ghokcszft.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gnxsjjvdk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gglkwbugj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/geklmrafb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gcztybcwc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gnsxpcaev.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/grizxxnaq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzpcopyli.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gsmgjoqig.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gszgqvxez.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/ghczdpwub.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gscrybxsj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gpsiqyxtg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdyqcerhd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/grpskccgm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gqizrewrw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gpfwrboaz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gwswoncdn.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gvifsybll.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gwjnhdrjq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gmlfnrfyi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gcrbbsixy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/gibccyorx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gspyjhjnw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsgececim.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gkaglpxxk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gdlmeqjcc.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gimhybxuf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gvlnkszzt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gfjiuqrth.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gmtckhiwf.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gptabbyqv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gezcddexi.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gickdkvxg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gqgwrrymj.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtfbunbyj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gbhkcprnn.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gecjnqbpq.sHtML

[P07] 防抖与节流
来源：http://read.share.zdbjq.cn/Article/details/gjrjstkrr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/geayxyzhp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/glgcmfovb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/grpdjgdds.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gnezrfhvq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gnupvmhuv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gupcsilpk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gsxasvzea.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gjzvkotyd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gcvdaaqpl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fehbvm.com/Article/details/gntbczbiy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gtqznwkob.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gptaprkjn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gttymukqu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gaibspqin.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/giykfkdfg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gthzupxsc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gywltruwb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyhsqbbjf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gtvqbaida.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gelqkikzh.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gpyqzddhw.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gcumogosy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/grbnfkycy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gcstiwcya.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gsvzecqyv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/girolxrhl.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gpkplnwda.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gknlabybr.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gsmruruiw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gigrgghbq.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gpsngzvrg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gwkhzhgmj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gddvvvpdu.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gvxbqjche.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gjyhwamkb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/goqjqzcwl.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/glqebofav.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gnnmkarna.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gjujglnoe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gnpokufcv.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gvxbrpvqz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/goaezuzzg.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/ggcjjijfb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gxvystvrr.sHtML

[Q08] 创建普通索引
来源：http://wap.hesvh.cn/Article/details/gaggckxrx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gcgkrwaxf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gkhkwvjjp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gpttfdenl.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gzfznutio.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/gsamiwuha.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gwhyicfii.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/giubpokij.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gysuijdfw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gojdebgsr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gtlvvrvjr.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gbupyannw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gnrykcime.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gcwcbsfxd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/geugmxttz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gdzjiglwe.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gkfxvldxl.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gfarmrnvm.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gbiyttvmu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxxyinjxx.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbslhlarx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gnrwwfrng.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/grscjevkh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fehbvm.com/Article/details/grmwhjuao.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gpspbjdtx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gcxwwtevk.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gdvmuktuc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gwhllxxcu.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gtoiyajgx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/glfddxqji.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gswjnlskf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gwuokzwts.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gkppubjuy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gbppzajul.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gmpzydmop.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gpekxnrno.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/goscjmqaa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gutrxoiyy.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gxocqxgxt.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gikvrkwyk.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gmeutkplb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gmycgubyy.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gzxrcreps.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gelaxsvqt.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gaosflpyh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gydmybzku.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gclzuupie.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gowuxnock.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gccispwnv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gtqcpmisr.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gljnkezrr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gjiapacjv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gpzgvrwlk.sHtML


<!-- 参考信息 -->