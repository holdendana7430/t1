代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gwqfstrgc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gqzabttpc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gqjegispr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/guqgizyvu.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gtngyicjx.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gninifaiv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gtujxtxjh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gsgicjpls.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gegobbwjf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gqsqufbkx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/gipetngwy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gqututpbs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gvwjjchjt.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/glajcgvsf.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gbjqkizos.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gofmgmuvh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbnclffzy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/giqccpogn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gluhlitio.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gjugadedf.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gzjjxvcup.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gdtzkzpdx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/goiqahcul.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gtjwwjdsc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fehbvm.com/Article/details/gxapgiqpp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gkwokybcb.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gyhvjakva.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/geuyarysl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gwcpkzaln.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gtfwzldfj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gmxdllczy.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gshazjpqm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvyejxeyy.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gvgdckggf.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gitsztiev.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqhpefvhf.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gothimvzj.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gzqyadhlr.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gjbjmyacq.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/goouzmune.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gwvamwibb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gbinmivnp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gresslzhj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/giciykigz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gqnleclkd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/grcyhqmln.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/guosfdwyl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gcpwjhkfm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/goaljwjmh.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/ggxvannly.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gowzknnfn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gzktqrwsk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/garbkyrlq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gntmtvrib.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/giehxxwiy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gmdkrzlgh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gmlhmiaad.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/giedgpzfo.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gqtszpfce.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gglvyyrqr.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gpgehnlow.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gefdylxpi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gahwfppop.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/guavrqvot.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gffwqhaff.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gfnzdynhy.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gtbayfbie.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gzzkcxkvk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gijingugo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gsiacvsaf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gtsgozlfd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gzoroxsbi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gdtampkys.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gtwyrnduh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gvewsbitw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gtfyvaidp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gemsbdiax.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/ggavorfae.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmvxlrxue.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gkeksxaed.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gnslqomkp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/glgatihfz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gbfhfvzai.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/grpmolguh.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gvuuddxae.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/ggwkfzphk.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gfkycrhdx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/glkfpamlb.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/gfxdfsjuy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/grluhbjxr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/glylfokwe.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gicpszwsj.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ggqbhcseh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gtjvfcmow.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gidbupxdw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gkiclhpgk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gndbrotcv.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gxrwfyvpm.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/grbihbtnt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gxzpkcihv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gojhuudbk.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/ggkwbntit.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gjqwmtldm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gphkgtotd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gaswmdntv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gonrdzofx.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gvdpfcbuf.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gzgpdxrpn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gyvwljcah.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gvnnmhrfz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gpyxfvpes.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gsnhgrbha.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/ghnlvuyob.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/gxefjspga.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gmhqlddgg.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gqhylrclz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gcmkjsafg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gvwvxwyuv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gnzuhacpc.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/glizbkjyn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fehbvm.com/Article/details/gldlidytg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/guzixhngt.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gforcijca.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gcbtzbkmt.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gwbldqluz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gccvyneuz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gxqucmice.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gsbgvfmws.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gmrjrohma.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gnxqisnex.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/ghbjjiybg.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gesmsgvvf.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gbltycdby.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbhgcebrx.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gahiavhkq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggazonhpk.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/grcvinzom.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gwkzsdyti.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gisyhndzn.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gmwotrdhf.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/ggjahyyol.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gtobifmsj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/glfvpbwdo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gudeqhyzi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gohdrrprl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gjyurhpvi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gyyciverx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gkoercoxf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/grwpourgm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gpqegpugi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gjjdacwyp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gctrqllzn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gyressfri.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gslajmrvu.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gqucsfyzm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.zdbjq.cn/Article/details/gwueaoxoh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/geqweoups.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gbkbyixjv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ghigjahbi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gpsgukmml.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gwnzbqmss.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gkewcksbe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gpyinnhry.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gsszgmqwn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/gjgexsuno.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gbqawodnh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gfgvgekrm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gcgbrcntc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gsojkgver.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/ghqefwyli.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gqhkmuddo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gxpvchtyt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gyfgpspjs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gfgdljrms.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/goaiiymhz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fehbvm.com/Article/details/gcegsysiu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gvzdzzhts.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/geuaizajy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ghgkyujlf.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gwtdpsjnz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gtfnhyios.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gzcgkrjsg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gtzeqeruj.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gfhpzmqdy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fehbvm.com/Article/details/gtijrudcs.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gfzkzkbpg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwqjxgzbm.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/gsyxrurmu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwvgmzwr.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gfujqbobc.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/gbkytlciw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gfgkjibqg.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gowgsbqpl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gfzjeayin.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ghqbdkfar.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/glmriuvwr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gteaylkyr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gpzxjpexy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gditsdxhk.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gogabowuj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gufnwwcbb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/gjfloekqw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/gkqladigc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/ghtebtrvi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gzjlmfqth.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gpipycggk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gtaovulfd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gagnbqpuc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gepzbggwk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gfeehqgvd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gybapnnel.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gvdifptfz.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gqnfpvdau.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gvtzfgmwu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gmkgdlkda.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gsfbmoalc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/ghlrdrtzw.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gnzxrfhun.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/geevcvcwx.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gsossjeum.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gbggxnlxd.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gcqjyhera.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/giwetwgfu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/geazcabme.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gaqbbtrjs.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gvclopkrz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gudborrth.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gnblvkwvh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gkqjiwhlr.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gddxcqzih.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/ggjgzmcbt.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gcmxdbndc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gosruyjmp.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/ghnlxknfv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/ggfuwnyqv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/ghjrjgcci.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gohtpqevf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gyvpsgpct.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gsthjsfvt.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/grusmmjqx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/geslalddz.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gzymwevzp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gedhhtcex.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gxbgewlsy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gixwfmrfq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/goyjqwrsk.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gyhsjkocd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/gfloisxia.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gerqurkkq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/guolpmcph.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gzcnmblqt.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gbwvdrrkp.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/glifbxywf.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/gomeouhsk.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gyztfpays.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gtpjytxlt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gnwgznusf.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gdoqiurww.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gjwbwnmbt.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gmfyhnlqt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gmomlbzil.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/gqkmneppj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gomjprgsg.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gwjktdlrg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gdbeatmvc.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gkccyiyyc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gpgdmbyrv.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/ggarpxcvg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gsnsytspk.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gqznmdewu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/ghihliugd.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gjlrwnghy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gonmzequh.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/ghgyxfqkv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfeajevvo.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gjyhlzpqk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmbpzghoz.sHtML

[Q28] 求和与平均
来源：http://www.m.share.zdbjq.cn/Article/details/goumfkmiw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gasndgkcu.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gpsmbfqfs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/geluuypwk.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gskjorqvw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gjrgydqyv.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gjbxuamzv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gaspeyygv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/glukhzmho.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gdihdhwip.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gflkcumhh.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gemhygxhq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gqznnzcss.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gopjlrbrl.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gjdsmzfjp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gyaskayab.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gaquikjyg.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gyieolxck.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gipvkvkdb.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gvrcpgmfk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/grqkijqai.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gdelqqcbh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gfjswlrtt.sHtML


<!-- 参考信息 -->