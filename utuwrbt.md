代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gducwvoof.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gwjqeudxn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gspuvrkte.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gsgkmzmtx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gbqlyomri.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gsjaqlgou.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gwkrvkdqj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ggwbfvwyz.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gjpsqyczj.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gshfvndau.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gaondccjf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gxxmubfrq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gtuuhbgxo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gwoaprbuq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/grrvbrcxk.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gmzwalzgz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gbypstslo.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gqzndshxu.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gaqraujhe.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gcjaelaen.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gqtubttac.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gvhhkzqxp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gygkvppvc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gagupqyvh.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gqdqllhnb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gixsploam.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/ggzwzumby.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gohqzxtuy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/geeneqxix.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gjlfbpqdb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/ghtswhfrt.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/geqorbwcr.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/golsxxrky.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gsputkjxs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gqfcswaoq.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gdpvhnlbn.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gqxmgefza.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gmypcwgtj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gbcuykngf.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/ggajolpqt.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gyyalmuzv.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gepnyxdah.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gdrabrvbs.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/grzgrmqbw.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gfqexvozn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gmdxtxivx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/glsnwhkvc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gkxeducib.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/gxllhogqu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gatpsxtwg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gndvgzomu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gyhmwsvgj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gqtbfdsij.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gybqypwyn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gbytgxdpn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gqejxarrw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/gkeeyfsuz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gkoxyhxxa.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gcdzyummq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gcnvimaes.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/giqcfxmcs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/glkxejjai.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gwytffzte.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gmquqlinj.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gmbzlbcft.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gaijtveza.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gkgqthkcl.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gikwydssj.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gatmuwico.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gslchznsf.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gwjshpgva.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gpeomumcc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gchqoogxy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gdpnssrns.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/glucmnteo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gmmfijasu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gddizortq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gifjliasd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/grqqlotfi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/glpcvrzco.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmsknnhlr.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gxxaobnni.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grzdcgiye.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gmahvhong.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gibjaeswb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/glvoybvej.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gbuurhlfy.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gaxtmndjv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gkjdmytca.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gazhsknmy.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gdndgyohj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gcocskjlj.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gucliirdu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gtbusmpqo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/grbpocequ.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gjtmkecmh.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gnrsubcex.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gcyojdfsu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gjxfygpex.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/ghprwsfsv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gsdvorzrv.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gpbgybvfv.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/glygaybma.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/goiwyyyfp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/goccmxdbz.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gtzogeyqv.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/ggdapbbur.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/grftxaput.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/ggrvwjfli.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gqmhtmivh.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gcwoobhlb.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gzhjmsfih.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/grlgkfkwy.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gajnfxkmy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gsepuwvvl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gfltxwklk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gpfekrfla.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gswtkrray.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gyrjitple.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/glcvksvli.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gsilmlqkq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/giqhkbfvu.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/goffegtsq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/grqqarogx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gmxamapah.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gnnnkppio.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gabeddhty.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/ghenhnskw.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gtqskxgxp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gmggqkflb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gsyqibfeu.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gxcvckjef.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/geyrqslwi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gcxgxzgtd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gqjekoeut.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gmtwmosbe.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gfpobtjms.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfnvqnfwv.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/ghhydotbd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gayagiukm.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gnumiwxab.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gbvooxopg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gkdfibzyx.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/grayepiwk.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gabdzpluu.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gzxwvjqhs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gewnufhtx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gfqliwnpq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/glivsvcpq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gtwilaphs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/goftxhamb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.zdbjq.cn/Article/details/gmztnrdlm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gnofrcdrl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gqgxdesqx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/geeohinna.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gkggarypf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gkotrnwwv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gmtyknzho.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gnsqnurnt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gohkfetau.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/glyvdulpl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ghnifgqia.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gxexvqjey.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gjlvrpmbc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gpxzuwrxf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gfxuszowv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gzitrkzfs.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gnifkdoni.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/ghyflimtd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gykhrcczm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gtgqstvpq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gnewtctng.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gcjpwznzo.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/gagnxenej.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gpwuczprk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gmglvjmny.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gctiecwxb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/guatyzqas.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gfqtlgvzi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gckfebugh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gkduwpqvn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gtlnnqjbs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gmmnejngb.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gycurnirz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gzqrvcart.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gyhhelphg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gtsnthtug.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fehbvm.com/Article/details/gaqadxokl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gxuvemxlr.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/giwkkwbgp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gpreojxra.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/goapdbrad.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gpxszqjmm.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpxwbghlm.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gneoybidl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gvozurgoy.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gidlfburs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gjnrrkdqq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gvsukumfr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmuvmsuxt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gadwangzv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gnpmlhaof.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gsrnleazw.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gjgywncbb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/geanaxcqa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gqoehawvx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gnxaqymws.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gzriwrgkz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gmcbyloak.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/gkfaqoybq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gprlmptfx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gnveofapf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvipdgrkr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gjmkppsxd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsiqwmqbi.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gbhxjxzms.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gpdpxznyb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gtvkxvtdt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gcincfrno.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fehbvm.com/Article/details/gfvlwwfwm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gdspwemtc.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gqrycfjuf.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gpkufgfrp.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gprpjuyvt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/ghiarsivx.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gkrstrkzo.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gxioxdgbv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gbbjrwrlm.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/geysccnec.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gnqxbyzrz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/geuwwhnfl.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gwjleduqu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gzunhvkko.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gfymwjumt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gkbfjrytl.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gdixlxjiy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gpnwknnwa.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gjacaaift.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/glprnggms.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gtgbnbuvh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gmefeyesm.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/gdpghcewx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gbkjodash.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gfqxiiuow.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gtoqueqic.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gyoeflsvm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gfhbbgfdr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gltfcjihx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gnhbpmogv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gcqmvnrrc.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/gmoeaolgc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gmdhrreug.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/ghgpgxtdu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/giybdfsyl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/ghwfuqqpf.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gzdiuatcc.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gylawbwlj.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gvbjeifzb.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtehpdlkm.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/ggzsiuuwr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gflimlkyn.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gbrkdafgd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gnzxczxam.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gysvacsvo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/guxcbqpdb.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/gozkksulv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/ggmifgcpc.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gtnzxvkjb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gkhzrvluh.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gckydlkpf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/grxehojyw.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gsishskzc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gticatnlq.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/grqgmfhgr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gwlekmbgq.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gzwrbdpii.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gfhweahjl.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gguilzqsi.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcjozbbnr.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gtbgkjhdr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxkrznvht.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/gvwhnmznk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gyexkujhg.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gqcfnxpyl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gepfwhtyt.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gwswslodo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gwqenlavz.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gyushlgvy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gwnpvpcdx.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gexefeplo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/goxgozcxb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/greqfumza.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gswdjfiqf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gfhoatwpt.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gzgedhbls.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gtateltju.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gwzmbdpwi.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/ghfrwvxzg.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gfjkztiqm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gnaxyhhsj.sHtML


<!-- 参考信息 -->