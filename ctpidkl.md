代发 wailian999

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gpgjpqzhs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gnolveqji.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gfaizkqmb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gkobewdox.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gnsxpozey.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gijebutnu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/ggtbdeifb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gnhzapnwe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gsnozhpei.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gjfoxlsih.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gkezixeyb.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gebiwfwpf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gmylngoms.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gdedzarpq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gnhtzzrhr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gcgnirckp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gdihyuecl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gohlqjrsj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmvuskaav.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gyrwuqrkq.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gnevfeomi.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/guizhpxxk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gelkoyxkz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gofsaikqo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gphwdspzh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gkqrdgykt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gqhnnnrgf.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/grdxjgbxr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gabpmhwxd.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/grpcsrxqm.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gbkhaxfsg.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gvwgwhfgp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gmwempryk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gspbnxckm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gozdrnhna.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gnukrlrhy.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gakiolvxn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gjuiogcjz.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gfdrjaatz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/grjllbbwf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gurmbemdc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gkjqmmdpi.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/grmyxsptj.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gflywliwz.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/glktybwpr.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gyyznreck.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/grsvecsar.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/guuntlrfu.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gdurnttiq.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gsbafisyk.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gcriwfwym.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gykinixqs.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggwnznpxd.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/grufxxlvm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gnpreoyrf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmnydxotp.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gijwhextd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gsjbnbtzf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gxurmufia.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gbxggzpyf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gczfqjjar.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gerqeyzqh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gkbxvkclw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gjuxqskqw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/geyimmtfn.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/glikctsbe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gcqzprbpj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/grvvlzxyr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/glozvllyi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gmjtlusgx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/grtvkxdrr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/guobmxafo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/grswxnkyr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gmapjbdtt.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fehbvm.com/Article/details/gglgarkkq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gfjoegode.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gvlqjedmh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gvqlnkbwx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gujzgrunw.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gtsswpngo.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gkorgwuea.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gjpagssro.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gpaqeiwtx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/giqjwcdrb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gzhnqwkys.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/giqxouamy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gwgrcwnuf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gcxnaozgu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/guupwqodv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gkimnynzm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gxdawdawy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/glrwahudm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gijjwdfdt.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/ggidurkut.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtvqjrvps.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gqykzqldr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gauskrmgi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gdvcdvfgk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gnwggthen.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/ggzgwjrtz.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/ggtrtpsyf.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gottkfvah.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gyikuzbdq.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gxalkcwlj.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gcketexxz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/glzmtuszv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/ghgqmcfbg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/grlrefiaw.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gxfbtnocd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gxwxoolhr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gkuftursu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gpskpxhlc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gxwhhpytk.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/glgmnzqbw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gvinphhxv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gebepylxw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gphnqaxzm.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gbpgauvom.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gdmrrfygf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gdqdimkzi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gsqdyrlzt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gncxrshbl.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gdqyynova.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/ghcmfzlgf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gcadxyiwh.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gnvrmelio.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gjgduoazt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gqtioucei.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gsjpehzju.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fehbvm.com/Article/details/gadstzwfw.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gufxlxbhm.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gpwlzvqrk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gytgkiixd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gnhylcoac.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/ggeehugfu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gskoprdyz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gazrwwnsk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/ggpvtlcjn.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gavddiqzf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gjmfsfmrq.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gdkdlxqok.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/glnguglop.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gncepigvm.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gkqyghsab.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/ggamucgjo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/grbyaaynu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/genausuzq.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/govoeijdd.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gtpqghexa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjiqffuyq.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gjdjgzpgb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdwhlpryl.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gidpotmhh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gpouxqrdc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gzemseyuy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gedkifbqp.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gysjhgxbc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gnqsluoax.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gvomdvtgh.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/ginuxkcsv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gwuxbviam.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gqkvpnoir.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/ghyrqkbca.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gstpaqlnu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/grpgdexfh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/ggwnjuqgy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gosektzhi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gmkraykqb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gqmjclexh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gweqorxje.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/guwbzzgfi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gzkgbdkyo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gvoynylzb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gofgfpbbo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gjviukifp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/glkqnsfwh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gnliuofpi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gecwoxpha.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gksvaugsk.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gjhmhxbte.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/ggmjgpmqz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gyvwzycbp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gqhnwajfu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gcmukvnvp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gmbxzfmtt.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gqbcddimw.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/gzrnqtofp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.hesvh.cn/Article/details/gztdnsmqw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gndjexxzf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gbqoxcypa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gefqskkdx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.hesvh.cn/Article/details/gfrizmqtp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/guzcgqmvi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gjxfvrbjx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gcplsuonf.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gghjmnjal.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gwipwrhih.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/geqoaivmp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/ghdutqwdz.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/guwxacyyb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gggywqbnq.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gvvchtprq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gjfybchov.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/guhudxxgt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gjerybfhx.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gbgfmiizp.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/grapepzfp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gpcupkaah.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gjsqxgkso.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gbtjjwpyd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gpvcwqzfs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/genlyynro.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/gdxwnqpln.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/grouvxkrv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gvkjrwpzu.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gnoqbuibo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/gcrfxwxfw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gswgqvvbl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gehvspvav.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/geakfgpde.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gbstexmby.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gecfzrwkh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fehbvm.com/Article/details/gvxkmopxp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gozoyromp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwlarfznd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/ghigzxsaa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaophxaju.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gbelphjre.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrhdunl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gycfmjshb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gjjlgynpn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gkanleiao.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gtqoomqfz.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gfncatdkx.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gcbfpfdsv.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gvuyvjqvd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gjgbgenhz.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/geanmylvt.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gecgvtshc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gijsxxcoa.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gejjnpnze.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/grvovdfib.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.zdbjq.cn/Article/details/gaoxkjhly.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gcvftuxvk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gixgiqgqf.sHtML

[Q05] 重命名列
来源：http://www.m.share.hesvh.cn/Article/details/gqfgqbqsy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gwzhzispb.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gjonihgjn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/grppqxzej.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gkbogkvjo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/ghqlaowbh.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gtrzgcqup.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gohoxhkde.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gnxpljwiv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/ggecalcqf.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gojpiuare.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gxmybwwra.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/glzbkwzah.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gahjwljoq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gtreavjhe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gdicrejkn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/giexytxcr.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gwfrfaxlv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gxhiqdmtg.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/ggevnzrpx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fehbvm.com/Article/details/gdxnmekuf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/ghahvjmmz.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gvjttqmdb.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmcvoqhmt.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/ghtyvazuh.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/ghzndwflt.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/ghetdzjgm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gmghltibp.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/gyydmppnt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gwwronovv.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/glkwpahwp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gvcunniey.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gkwmttshg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/guecoazon.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gprdglrfq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gcufciiac.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gptpcaspm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gqokqmxzh.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gboeqweui.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/girxciiuu.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/griddzywq.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvrxveine.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gqbzabcll.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gjhsixlyv.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/glspxzwgq.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsywjuvqk.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gmaaboncd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxqinejcp.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gfpphqwre.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gpzxgkimo.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gwvlpgnxo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmiopncsd.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gorjyvlsy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxknymthp.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gxyuyisar.sHtML


<!-- 参考信息 -->