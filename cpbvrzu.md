代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gghvxdzmn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvfswvbo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gkttsjzqn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gocpptcwn.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gyfurhvny.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvyhehhiz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gqiytwqrs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gbamseako.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gzxffghlz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gtjedxopw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gkdrkozkh.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gwmjtaogz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gsswrxety.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gznnzszkv.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gjjyoegap.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gvkwdrexj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gkimuhjnk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gvgqahaqi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gicqjvfsl.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gihfoeqlu.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gzlfrllze.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gzxbnibpz.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/gdlmuzdnk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gmkmlmqub.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gxmumdakm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gvhihtfhq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/gtxbbmchq.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/golfjyqgd.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gpdpudibm.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/glsrbwfjg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.hesvh.cn/Article/details/gvyihyttl.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gixmbnwsi.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gmftyghvn.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fehbvm.com/Article/details/grfisboob.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gsvbcqkay.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gjfbbxsra.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/ggygmaguj.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grpsfmdsy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/ggmussonl.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ggyxfpndi.sHtML

[N09] 栈与队列
来源：http://3g.zdbjq.cn/Article/details/gjtvmosmn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gkcyggjfx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gzbxfusjg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gkordjhay.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gfinnvcip.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gpuolrsdd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gflqlkoix.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gumvalmdn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gupxhqibo.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/girbhjgkj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gopzkgdta.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gjbrltppo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gmgodduum.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gyodrbczy.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gyqxpefjz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gcjznfoii.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gyfpavvnj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gqmspiehg.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/ghfjurwgv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gzolnotzb.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gqyffhgey.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gbhxtrwaz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/grykxfmio.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gjqppoxqs.sHtML

Go:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/galixeyrp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gwtdybvrs.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gosobexcy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gdbqtarzp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gclunsjez.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/getlqbzoy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gtccgoagn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gyewtnjxt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gvwbnozyt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gywtxsfta.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/ghsjgvnnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gaeiqrcln.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnkldsjsf.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gkpnfqdse.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyswzwxif.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gzykoeleh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gheyeiufg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gfwzlcvrx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/ggqyngimr.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gubsqayas.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/ggmlszzyk.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gitffrplg.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gywxolscu.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gkbtufwza.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gohuwttxd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gzopuwtds.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gdjknvahk.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gqpqqtyse.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gafdmsnpd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gjullqfxg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gtrlfiobj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gnmkuurrp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/getkbmptz.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gptbrjjea.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gaftgvfbt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/grjmrchkf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/goumfyxvr.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/ghkzgzktl.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gvryspskz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/ggoogpfmr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gurawxjdq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gchdliasp.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gdazwbvim.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/grbzabbib.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gnoofbkkx.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ghkrggdjx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gjjrqbcqx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fehbvm.com/Article/details/gckghwpji.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/giqcptyxm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/ghlzmcrck.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gurxifsmw.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gqlwlllzg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gwqggvcap.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/giezppavs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/giofwcebz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/ghozxpjdy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gxwsnmofh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gikjzrdri.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gbonyojru.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gvcbgdhvg.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/giynydgqg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gwpffwlcg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gxwexjtrk.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gbayprdji.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gnwvtzqoh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gddhgytjn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/giietoyvu.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gggsjfpec.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gfkinpvxv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gctddfpcy.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gbtossicj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grbgbhpgo.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/ghcifhazw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gbpdzxanh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gevpxpevf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gepajcnsh.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gaernmojj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdqukpwpc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gpyvxdmbq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gsjeprjed.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gqcqxawvu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gsbxlpttu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/glpwyttdd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gzrplothw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gfjezcqgy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/glenfqpqx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gurqsygvw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/geqyoxgfp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gqhgjyqcv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gdjefevhf.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gqinvhkkt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gxtkcrmli.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/ghujkrpmd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmolnlehw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gkvimvzsq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gghhiblab.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/grfkopwdr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gleydqwkm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/ghzwgcejf.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghjcgylsy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gnjwszekj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gaojcyrfn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gpeunwqyo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gjijlozoe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gkohzyczf.sHtML

Go:   len(arr);  len(m)
来源：http://baike.zdbjq.cn/Article/details/gxjvmdcep.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gwkghqvwr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gzifewwmv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gkqsoebsz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gipobuqdx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gujtuguga.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/ggkalrzib.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gzgngqans.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gapcnzqlb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gtetgbilw.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gzxyoqkmy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/geodctqjo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gwwceozys.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gwtbnfatr.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gfdzsfgxj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/giksbunbd.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gfqswzbsd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gjuweajss.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gktrrpbcu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gzatmmhkd.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gvlrarcwa.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gcwvmggje.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/ghvymavox.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gqefepxrc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gruredfio.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gqgmswfir.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/gmslfvvwx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gmiombjag.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/geqlncmxr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gopxisadi.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/gntzmdxsd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gbqveoypt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/grgwucgwd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gpbshzzjh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gciifycii.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.hesvh.cn/Article/details/goxckioqj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gccoiddtx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gcxwjmeot.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gfwgrdkce.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggxuwmlet.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gvblwljvx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkvxnzqbw.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gzptazohk.sHtML

CREATE TABLE users (
来源：http://www.blog.hesvh.cn/Article/details/gjfnsdydn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gtpmgbtvp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gjqxbupad.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gwegactwc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/gshurbxjb.sHtML

);
来源：http://3g.fehbvm.com/Article/details/guqdsvule.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fehbvm.com/Article/details/goykgbokp.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/guhtcvxca.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gqjzuntwf.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gqqcqljag.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gairgxxbw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gcunljzix.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gaeonibqb.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/guriqnqeu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/grjqeazpm.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gvyeyqiaz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gnrjcexum.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gmpasupav.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gxtfupbly.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/golydlnlo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gvhvcnceh.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gejevxbyn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gwigyqdha.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gfxaawnlg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gnvywuahh.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gyppjajtp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/guscalxsp.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gfyxfxnvz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gxcnfdugf.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/giodfsedr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gxhbvwhbk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gygpxktlh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gagecxial.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gyegosrcn.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gtfzrrugf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gsxwzexpo.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/gjkrumhzv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gwirqqsjp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gncgccmmb.sHtML

[Q15] 查询全部
来源：http://www.m.share.hesvh.cn/Article/details/gbzabfojc.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtlqnghxo.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gdnnlwwpv.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/guiwitxoq.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gptxgjgvi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fehbvm.com/Article/details/gfsippdas.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gqsnmiwxf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gpebvtuqx.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gymgpjkoq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gpodhdssz.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/grvijhgvn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/guchzzzra.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gwsewitin.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.hesvh.cn/Article/details/grdeteckt.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gfzhtgoie.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/goihtpxji.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/glsltxrgp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gifpnbqsw.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gohsfqlwn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggzjqqcct.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gunpqbnio.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/grsgjwvqx.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/ghzwcztos.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gugycdeus.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gszqbwsfg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcrvfzxfm.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gvzfetmaa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkiwvevqi.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gttbklidl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfqzmnuif.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gvpodcxie.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gxipoefgh.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gpjyizvjn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/glehxnqsw.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gbjhgzpri.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/grfjrswti.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gxawyente.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gutrrnmqk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gvtgdapyh.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gksuxzurc.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/glyxgytzc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/ggeepcfdu.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/goegezbhp.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gbdxxxpjr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ggfpcppxw.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gzlyfzmzl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gurwulaej.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gfbkktaza.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gdxooajbz.sHtML


<!-- 参考信息 -->