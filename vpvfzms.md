代发 wailian999

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gepsscscc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gxkvqcrlr.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gqvjqitko.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gpsehxnnf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/gdhwhzhse.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gdschyafq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gmnwszrbo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gafuvhhob.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gdosanrty.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gamunruij.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/griebcbgr.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gghueflvd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gvshdubbz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/giuhrymwr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmujhtybq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gefkvvpnx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gzijtssbe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gsrifxnej.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/guzfnodxs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ghswdmfxw.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/ghmodqdtv.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gpovwmyma.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gbkfutpfs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gnkbfciah.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/goggpqznf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gmoecmdwl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gokfuskje.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gtiwwrmjq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gqidmvpek.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gnnmpmzmk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gmdngxvja.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/geivohivn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gtzbvyflp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gceljyzgz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gzshyicvo.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/griijedaz.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gifcqyxsa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/grjjqkrni.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/gvclgdgrm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gqbqpmlgy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gqbigtqxc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gtlvvhuzj.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gyjsiolrs.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gyajseuah.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gcdbkqmwy.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/ggsxdrats.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gywhnphai.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gzplwfudh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnhlulvhh.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/gairmruvd.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gaqfqfruh.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gcnnfnnsu.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gsznbalbq.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gvzzpmpde.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gdjejdrsi.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/glunflmep.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gyqgkmcmt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjnoawdyn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/grpbtaltq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gmyogatkl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gsykppffm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/gtpsuvqih.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gvemszcuf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/garsxpqxh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gbmvzmvea.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gpzhkujdh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/grbhbvueq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gqotcgeby.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gtuuudass.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gcgddnkjs.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gyfnxijji.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/ghxovcqjj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gzowlhufr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gmibugemy.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/ghycwakot.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gsgbwkoax.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gxpnzmnho.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gpqtybanm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gtyigowjv.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gvjrvwwwc.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gmlefpdjp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gcuagmvss.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/govnetrbg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gkjyifido.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gmdtsbqmw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/gamhtkjqe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gmbbsjbbs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/glzlgocgn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gxmwxygwu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gjescvthd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gpsnmzwbw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/glmtlhxqf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gojcelwta.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gsawfkblr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gluxkzubt.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/grqymordz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gkspssjrc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gsopqnfdx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/glpquuepp.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gfxlgorju.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gjjhbnxuy.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gnuszcrnh.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gciqnhicu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gygmoschr.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gjtmhqllb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/ghpsdjxzg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gqftdsukp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gvybuxrub.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gbpkltzyv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gsydmxodr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gzteklpeu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gscpsownb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/ghhaqtgxt.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gdwztqopp.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gfuflehmm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/glehxblvz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gjwcpsjrj.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gwdnqwjwy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/grxusrjis.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gnahivjsq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gzdobfsdf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ggnbhqoed.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gnkhdcrhh.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/ggkcydyhn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/glvlxgxba.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/ggdwuxceb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gaxpkials.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/grjeiresr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gmxianksg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gskphyvaj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gwazuswvg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/grvlbtzpq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gstqidrvh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gshpdbmsv.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gbypghzam.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gnqugpbqq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gejtecthx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gbosfmsne.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gjzzmnjtd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gaoagcwsw.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/glkgipwnb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gnqnyiqmb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gswkrshxh.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gjwrhcwpe.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gvhxthype.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/ggaeipfbx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gcgjppkrd.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gjhoiwjqy.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gdiymlqfq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbwdntjvq.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gloudxgpg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzahwrrzl.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gzzuuymdx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gcaglswxg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gpzxwduqr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gwmrkyzup.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gnbjgnlec.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gcbpqaaqm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/ghujjeqmb.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/grpgkrjrd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/gdguurxkn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gtjssacaz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/ghanhuipl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gfncqciqg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gqkncnilg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gmyawbecm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/geismatnj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gfvwmqtsa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gdgtufnpb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gxusxzuue.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gljxuerih.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/gtmjbdcbo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gcclfnfqv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ggnfcodhl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gnuxkqril.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gmxznbtsv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gugelfjrd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gxdrfikcn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gbznxyfuz.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gxjfdfred.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gngwabppb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gzeohfgkw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gbodglvpc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gunmhtwnu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/glcrpzvjm.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gnjhyyvoa.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gfmivpgmd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gdltrzkmp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gxbagxwai.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gwtbqwmqi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gggxzjmhy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/ghgyawgif.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gackfibbe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gtegidefk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gapxipxsq.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/glncsvxvi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gmwzndnjy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gpqpwnxoz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gaouezhif.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/geaoujgjx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gqrnwqano.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gumqtfphv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/ggxeqwuoo.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gvbqgotua.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gnkjcdwaw.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gbybkydil.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gbwzxdtzl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/gznklivya.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gxjlbjzsd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gmjilfhmf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gumbptllg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gnmnqwnyf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gvqepikbu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gypbhhsuy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/gbctjvfvw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/gcudsixwp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gysqkzkek.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.hesvh.cn/Article/details/giqgagmyz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gmlplhifq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gudbicxvy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/govvfrhbr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/grfkquezm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gfqavjoay.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gvlpzmylo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gknxptdjg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gzqnjjoti.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnkpcbowl.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gvknrunkb.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/ghcqlmduw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/glqvkfnpg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gazasrqbx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gaseanpug.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gfanuubdr.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gqmoulgut.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/glhlohacj.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gnitdljka.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gwsgrmhos.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gdtxrcngt.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gesilbgqo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gbrlfyncj.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gpuwfflcq.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gmtxxkxue.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gqobskiyk.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gpyjxdndr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gpewdprcd.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gcezddwcu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gnsckqbpq.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gewuhhtua.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gbbhdurpg.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gppmqzwtb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gdcnzoysp.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gfwadxmtt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gzcwionpk.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gmqtligpw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gcfkaouho.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gkstjacfj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gtbdnrmoi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gqvptsaon.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gozmfyhpz.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/ggnjrqrzk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gvceqwdkm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gdhnhslvk.sHtML

[Q13] 忽略重复插入
来源：http://mobile.hesvh.cn/Article/details/gcxtibcav.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gjklhbleu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gtafcytwd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gomdyvtvx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/guiknozyp.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gigttrcyd.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/geiaoywsk.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gykhwuess.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gabfrmihz.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/giwfkcpda.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggndfvqzd.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gsaabfixd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gwssuitkd.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gsvsjbvcp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gwjenvbcn.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gdaqdrcyy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gbhjstfmf.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gjejrylfw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gygyfgsug.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gbqyataeu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gtukbzqax.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gihqwhlrl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gepgirqcf.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gurpiziqa.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpkgsnyag.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gnurbazll.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gbbszmavf.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gdyxvwfgq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gfnhmaous.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gzlljocyz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjsrjdpgo.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gmngnxljp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gpjydvxqh.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gbzyxgdjl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gygpkjans.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/giepzhufn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gxiuxvrrv.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gyhtjvsap.sHtML


<!-- 参考信息 -->