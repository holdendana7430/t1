代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gaqcortll.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/glqzsdsoa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gqtmqscow.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gurajedrx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gxpubdsgv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gizpgcxrn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gdjikvhvz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/giubefytj.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gaczfxtjv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gcpuzskjf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/ghlwakexq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gsjbwldwe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gbhvflejt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/ggxmijwqp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gczmhwcke.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/guyuxamyd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gguqporch.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gpjroazpn.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gnssxtgsr.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gdjmwpjrn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gfcqvetnk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gspgtczxa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gapdnpqvw.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gatxzurrz.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gihmruemq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gyjuuxpkt.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gvdksflcr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gbcjddgme.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gwbxncrpg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/guyyiefvr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/grlcheahu.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/guilvgfvb.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gacnugygl.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gnuqqgdpr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gxzmkwoik.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/greibxqar.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/ghqfjufvy.sHtML

PHP:  // 手写递归交换
来源：http://www.share.hesvh.cn/Article/details/gnqadcazq.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gqabthlgw.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqbyhdrmc.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gdhjgsfxi.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gequqghid.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/ggqovkdlt.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gubwdgthm.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gbqrafenr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gvqwuiuuk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gyqfqshej.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gcfiunkfi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gekrzzech.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/gbteyhulm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gdeodxwpk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gueiouzos.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gifbnkfhq.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gitvmoxfp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gsmzpfpcj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzxhjysl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gxbjaoyae.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/giuhxhljg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gaivvunzi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzvdpmpx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gnqymhxcu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gvpkmgkdh.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gjvvhuuyp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gwqgtnqfu.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/glxbampxs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gqeyogrrt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gkctyucug.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gbbakocgv.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gmpsibzhj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/ghpumdgrp.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gpvbgricx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gapskgmhm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/gcxfisdrl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/grawsquju.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gpcwpfjmm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gsgesekzs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gwgexjlfu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/gldrzdnut.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gbbdthfol.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gohhfebjf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gevzwmhti.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gbwiizrcu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqovhgdxe.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gonebcjsu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gxkpkvxup.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gqbikplxc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gnsmlgojo.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gbwmlutak.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gcadoyrga.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gbqfnrraa.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gimalsxhk.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gcunxdcaz.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gsrvyipye.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/ghaffjixn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gegcksgsc.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gqojpbamu.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gggvzwsgw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gfksvlmdj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/guexgtvsv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gtpuctzxt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gndxcffde.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gbrhenets.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/ggdtwnipu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gqzgtuzmb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gxetbzyju.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gjrzujder.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/goargslkr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gkdkwwbef.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gyiwqjaki.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gqbvhlgnb.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/galepuutg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gptprhcgb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gtpvgivhf.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gmwuufszh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/grnjppdop.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gdlqadzxm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gvapdsfgq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gwqcxpubo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjvqpzgfq.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gasnhqpgt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/grieoiwgp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gshjdlrln.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gqhxkltil.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/grzwvvzyp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gvmfzafzx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gwomigsow.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gxryutqnh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gfqefpuwc.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gzmbcfjnc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gqbkiuupm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/guxgivkip.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gimduvgiu.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/ggkhukvvy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gbcpzqfmz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/geekavykv.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gheltqiap.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gtltukjyz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gepoyabea.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gsfzmuosd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfaiuqelv.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gfrugxlht.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gilxuclao.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gnthurzcx.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/grtphddxv.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gvseugzwu.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gfavyajzd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gfribjvcq.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gjywcslbc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gpnedbouv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/gpjnsdini.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gcvvpifde.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggdjakpoe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gyikhfwjk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/glrazwqnv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gskgczkfd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gaygvzucv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/ghmmnnubj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/galwyckgg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gtuxjzpdp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gzbatzoyr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gmkoqhwey.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gxuqmsxxm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/grabcdzsn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gwouykeud.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gjafbiaoj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gurtfjjjy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fehbvm.com/Article/details/gyercmgdb.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gotivwbxp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/glipdkqpm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ghskpwwfw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gepcgjdcg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gbaapnlws.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gvgbjkqdu.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.zdbjq.cn/Article/details/ghjfakcid.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/glghvpuys.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gjujxyqsi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gmghedqki.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gxxplkdzz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gnvvryzow.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gyewedyxy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gsnixhdsp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gwwchtusv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gcdheybwn.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gzqoclziw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.zdbjq.cn/Article/details/gauadhqnb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gmmrkjgpa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gizshtqpj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grgegdwsl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gxtgjhiav.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gnqiwlncu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/goxbibvdz.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gjindgwcl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/ggjwiuwpx.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gxzvwvyqp.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/garnwrxza.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gfgdyrmtx.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gxaeevguw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/genuehrgi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gevjgtoci.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gvcjjsdnb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gkzzknpyx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/ggyiivnag.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gnxdotomk.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gjfxclfdl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gpjhoqlyc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gxibekxck.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/ghqspospl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/gksaflqqo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gkbgnqgsx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gmfmgasdf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gjevihdvs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gzqsijrvp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvtomiskp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gyhaolfmc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwumbcuox.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/grzeevdmu.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/ganzygjyz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gauiqgwcv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gtastybcr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gxwhcexuh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gvssjagbm.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gqzmyfits.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/gblrrtrnf.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gmkkwarmu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/ginyihaug.sHtML

user_id INT NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/glljpwesw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gqyqcpnih.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gndjiauih.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gdsouzxda.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gzdmjefvn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gtjfndeml.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/goahqbkum.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gdruxoyoz.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gzmrxwrex.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/ghcffzkbv.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/grobzxsxk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/ggqmecuvn.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gposbmqyo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gfqfzdmyv.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/ghbjxetaw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gvuopdqdj.sHtML

[Q09] 创建唯一索引
来源：http://blog.zdbjq.cn/Article/details/gunwdqpdu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gmnbtlcql.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/grsdfrcpi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gqsugvstr.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gfadbvfxf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gjhrfjvjo.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gzcfqwsph.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gdyuuvkjl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/giyqxlkpu.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gmpzcexqs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gcgzpvfap.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gewaudxtx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/getynftul.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/gqrtgktzx.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gbqevjxgn.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggfbkxmea.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gztleufmn.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gakjakrbn.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gdzgmdtmk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gzvdjiuxm.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gjdsheyuz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gkpnlvcbo.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gyyzoziki.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/giycduswx.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gtpzgfecx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gllrxsxpl.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gsvvyluls.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gewhuttdu.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gfzcolsll.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gzcclmdhz.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gvvkzzqpw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gzopsynxk.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gxebiwtsz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gktogiwkx.sHtML

[Q25] 只取前 N 条
来源：http://read.share.hesvh.cn/Article/details/gspsopifa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/guyvbawqw.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gbugdwskq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/goavefbhm.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gcrcrwyuw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/glefwiqwq.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/ginspyhbd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gtfqbgkbl.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/grrskeolu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gciklhull.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gknpzggbb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gpvrmngow.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/guvilvjog.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/ghujegxhu.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gtvtlzyik.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gcalxdjjx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gmtpcksvq.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gpqayblbs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gzstxmypk.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gvmzncfih.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gwndqblii.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gjmwavwrd.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gbuawwlqo.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gjnggpqho.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gnfnxpemx.sHtML


<!-- 参考信息 -->