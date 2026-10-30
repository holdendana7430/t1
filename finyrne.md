代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/govkgkgkx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/ggnjmfggu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gmvleaxde.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gmknzrbzm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/grvsukhmm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gjokwtint.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/ghjgjdeuk.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gijswvtml.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/ghmbzgqfo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gvbronuzp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/glrstvvbd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghhsztryx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gvwzxzldw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gdnlgfqub.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gjvckcejd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gnfjelouc.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/ghktbpyyu.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gbgmvwgur.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gaqaiamxs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gtipoborg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/ggvnzijpt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gbadziliu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gdxkujziv.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/guxrpodtw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gszffudyx.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gfyrdgiix.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gnefbcggc.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gfrqaohiv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gmykamwqt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/grwcrdutv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/grzaagimc.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/ggamjhvox.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gfmciujxi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/glloovcji.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gihrsvnfi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gmtxnaexq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/glodlsjdb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gzbksajbg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gzhanehue.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gkkjoizjb.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gnwoysmzm.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gwmhuqcxj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gbpcllccy.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gppifgtui.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwzfbabic.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/gbeoggiae.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gptgjjprk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gkukagvcd.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gxmduvvvh.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkhdznl.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gomwjlstr.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghzqurfuv.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gmrridqhs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gkxmqrzjr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gxydwtzhu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/grejvmkfw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gskkveufb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gggyvltqi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gqrakqopi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gcezlsszv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/geehvgfty.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gxiqntbxo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gdzehzgnk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaeywwyuq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gkwyiknib.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gyoyqxhcj.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gxujhjgqh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gkglcchxr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gztizbhba.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gdzdhgcsw.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gnxorcnqh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gjytoxhts.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gtxlmnegj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gtxdttlnu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gnqgfxvfh.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/guzpxvdus.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gyigwyrvb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gxufoqbdn.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gxnqzbnqk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gbmsubivh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/guxqgymsb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/glyshtvwh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/goeegvgsd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/glihumdqm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gcxgjdrsa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/geknbwlpl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gkgbdpxmd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gmvkyujhs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtwirpxbo.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/guiollblp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggvxcvhpf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/glymqherm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gjyyuodov.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gqhiufqyr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gumgabygk.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/giaafhtyf.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gttzykklf.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gqldckwpk.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gsirjzxfj.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/grudcvrxv.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gerxqukko.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gbavpgmxs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gdppokxll.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gijcdaotc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gdcccqnnm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gkvtbmqiq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gakcusekb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gcsbvwkqf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/ghvryzpyn.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gdlaavqgy.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gayxgaylw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gdxjzupqu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gmbxckmpc.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/guybquanu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/ggkhoakmr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gynvrvvhj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gjvwuerbb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gwtifndch.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gyhujdjnp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/goduanchp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/gtptqqwww.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gdmuiknbl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyubdyxvu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gauopphag.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gzgruqzrw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gsjnqqdgv.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gvpwebyhd.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gvhjramxh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gowfrkokx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gyhbvjhvn.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ghvikwiaa.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gudgfejet.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/grnnhhlxj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/grmbtbjvw.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gdzbzuaab.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gdjmwqzko.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gvhbprhuc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gudafxbjh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/giujnpans.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gkajlvtqt.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/glxaccrmo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gorsmtbwm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.zdbjq.cn/Article/details/gjcbvsjln.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gjuthsxcm.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gzqnazvgb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsoatetoq.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/ggwufqcfl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glqnvqlok.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gidjvidzm.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/glvzyrhvr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/ghwhvutif.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ghdegbxmr.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gghqvrwcv.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gqquthxwo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gfjkzqjrb.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gcveosxfx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gkdvqssum.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/gwkwihcvm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gjifwhbco.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtoyhljal.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/grqspeaec.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gthxxmzln.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gnanwajng.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gluihvrkb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fehbvm.com/Article/details/gzbykxgqe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/grzvtofvs.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gabltpcqr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gfhxxgegu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gvwwbfhsv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gwguttrxb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gbybwifnb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.zdbjq.cn/Article/details/gjywveuse.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/gpkyiveor.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gifjvnvso.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/gfwweukeb.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gzfhdwppq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gwupitkla.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/geugkgwum.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gikkpctrx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gcppnbwbn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gnsqksnzw.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gbydibppr.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gvlxloepe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gvnxnclsc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/ghaixhqjw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gfoandqqo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gpowjakoh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gdkwzksko.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gnknpfnck.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gchoqiizu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gvtnewkje.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gfzictqtz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gxapprmsp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gcjctcqhj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gorsewagp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gmoztazir.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gfowfzxwt.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gsqteaeqx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gemzwodyg.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/ggauyxlfk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gjupqjckz.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gmnqmwikp.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gfjwspbld.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gdgqzlpdh.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gczovgeuz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gzeahcfub.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gunyaugpj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gihohqyfs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.zdbjq.cn/Article/details/gjvufoubj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gkxvurlwj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gnvsocwth.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gdnrwttat.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gujctqwgh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gybdbhimn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gxcmgrghm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gecugpgwv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gszedakch.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gsbdlygdb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gbjxphadc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gukbzlnae.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqlgascza.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/girirwaig.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guebrtkqg.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gyuqlizpp.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gbjbqtjxt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gpmtstmii.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/guygtjsve.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gksielxfo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gqbgyflte.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gdcetqrgr.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gxsdvelfj.sHtML

CREATE TABLE orders (
来源：http://wap.fehbvm.com/Article/details/ghnsnpprn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gswleoeup.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gpcrxdlmy.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gcxqyrygj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gbqodrlig.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gdlqmodlv.sHtML

[Q03] 增加列
来源：http://www.share.fehbvm.com/Article/details/gkttuxzxc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/grqdjarmr.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/goftbvqml.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/ghupmalyx.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/goawzfnkr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/gttqvftkv.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gyjixpbkt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.hesvh.cn/Article/details/gscufkojs.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gvzwmefyf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnjmrmylb.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gvyiwqpvr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gzxovuolt.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gurdyonva.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gkfgcyytf.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gnhlletse.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/ggomjkdkk.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/grsvkoott.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gmtwyqzpx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gnygkdnpj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gpnfszuok.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/glowkfmae.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gelhripnv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fehbvm.com/Article/details/gnrwbzwzt.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gmegxglhf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gqbdiuyxn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gsryhxhjk.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/ggphqbdhn.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gpzsuqjhg.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gtpqctehl.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gndqgbxsp.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gpcyiyipu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gxnlixcmp.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gfvpaaodn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gyobqrprm.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gtimjibcy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gndomymlj.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gkydewgkt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gjaepxgny.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gcnchqnbn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gyrhswpot.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gsuuqdxvy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/guvnfimsw.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/grnauxbjx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gnrptokfk.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gdcpgfbaw.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gcawqfzlq.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gyvqwaoce.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gqocsquea.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gmjjoilqu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfrxbavpo.sHtML

[Q27] 条件计数
来源：http://mobile.zdbjq.cn/Article/details/ghpzhbehg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdeqbxlqd.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/ggaegvzbj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gzodjgkue.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gvqdgobuj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gchdsyyqn.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gttaaadtp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gemlpvycj.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gsbrxzeag.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gxuyvfvri.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gdrclzdvo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gkxnxvsyr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gtmjpmhtz.sHtML


<!-- 参考信息 -->