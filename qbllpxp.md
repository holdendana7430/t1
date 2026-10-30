代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gkumyfgtx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/ggeqfgdvc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/goaakhtwy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gareohfzy.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/ggyepkawv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfqjweqwf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gprshgaey.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gseilipba.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gnrqsngzj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gwpetxphw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/ganslovim.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gufkisxxi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gpaoznbul.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/giwmuwqbb.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/ghkatnzsf.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gzxfvfqaq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gcfyuwtnl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gpkfhlvej.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/gtcpgkhzx.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gxdkcwbav.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gguexrvro.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gveoyjsgw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gasxbuhhz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gudkpgolu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gvulfoefs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gitibaybm.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/gcoslmagp.sHtML

Java: // 手写 HashMap
来源：http://www.blog.hesvh.cn/Article/details/gjetjlzxi.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gahgubube.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gwdojfkmb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gmvsoypcu.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gbcfxzbrl.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gfcytuhkb.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/ggqoctpme.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnvghrnby.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfhwvisul.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gihqjmban.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/glsikfzib.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gxwszpptw.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gozudnugj.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gxtdsxspn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gjooyjkoh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/glzsqetig.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gyhbzmpgf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gglbcmxws.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gcylodrws.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gqczqwmmo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gbjlqexzd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gzfexbigl.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gzfnywjye.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/grhvrjlxo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gnfgvejly.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gmyeqtfxc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gdqadrixl.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gtgltjrah.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gpbwlqery.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gdcklyakq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/ggnnfoamf.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gbpajwvlh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gemldjjrl.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/grsojrish.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/ghafpfgcq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gxkaamxwq.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ghvrzqjbh.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gtckortxo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/grnwexfre.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gbfmbrtvx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/geqntaexn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gtabqdydq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/glxelnvke.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gsayoxhha.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gltamorxc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/ginwzplss.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gqknxcgce.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gxdrcijgx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gbfsjmfce.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpnvywgaq.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gadztdrhq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giljwfunl.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gphtedrsy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/goqdldawz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gzceeyvor.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gmezskxgs.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gkmnxseuy.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/goxperxju.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gpjaqtcxv.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/goalgavkr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/gyxwpwcee.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gokmztrgb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/guzeuadrr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gqtywzumq.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gmhoaelev.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gmflzhbkk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/ghumkjwoe.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gefybcabc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gxsujieap.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/grjaurrhx.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/ggpopsxxf.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gvhfikqew.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/golengrtg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gilzubtjd.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gzclvxkwv.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gtlosooli.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gozcxbqon.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gaepkxjft.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gxfbdiggb.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gyporusng.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/geheibkgn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/ghhmdibua.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gjrhjdyai.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gphnbizoe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/ghqygluiv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gjqcqtbya.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/grmcftxat.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gedkuehag.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/ggmxfwatp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gpphtanjr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/giudummti.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gbmsxikxs.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gbuzhgagb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gdgopauvd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gprjlpkwx.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gbxbxrndg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gsolgcfby.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gwnwujypn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gcsepxvqp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/glkrglkue.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gdxczaorr.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gujnetrdo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gbwdyylzp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/geqismjmf.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/ggpmipiko.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/ggjndaqrg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtrdvqhcf.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gcloijcqr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfwutyjuy.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gonnkmjou.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gcjjkqabx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gheaclwvn.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gfmbqfqej.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gjzrdrqep.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gjyshddxu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gieefsksj.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/gulxdgvou.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gfzseplge.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gcgibpxsx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/grlhmvajx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gnfynncpz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/ggfbpmbfj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/ggihbheme.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gqdkqcqqj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gpyrvycwb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/galyfriqx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gusagsujn.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gchivmvsk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gucbwqywa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/glxxwpfrf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/ghgwxdval.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gjllffytf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gxouqmhab.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.zdbjq.cn/Article/details/gfybcwjov.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gnnhqhtqy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gvqcfaeoo.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gualyeryp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gdmfmwacp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gqbctsmjm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/giphmfjxp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gffxasydj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/ggrtvabyp.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gkxgukfeh.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gwydtapzk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gqtjjqmpe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gszbkvqly.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gqzxyvdfs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gunfnfbwg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gssqrrfan.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/ggknsrcfw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gqdfzvaua.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/ggitfqhsa.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/giuijnxlr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gigxaupaf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gmrqdwipl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gwzgphlhj.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gbrbzcjsa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/genxnjhje.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gzyqxpuew.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnhlwwdcg.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gmxywkpwc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/ggvwnjkcz.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gjhvsqqla.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gnkjdfkdr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gnzhmgfvj.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/ggojkyiwe.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gfmtetnma.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/goznklrrw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gwywjwipk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gcxdzqazm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.hesvh.cn/Article/details/gwxeosvjb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gjikhcgqd.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gwmocefim.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gmdnzcnzy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gwvdnvquw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/goqyjquvi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gevydetyz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gcdsdqcch.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/ghamwnbbf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/ggqdnihsv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gbemdmdah.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwutadhnh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gfojayhuw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glegpldaw.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gqgwccwhs.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gtessiysv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gcgffcbjx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gocbheuzl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/glxkdrwdt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gopfraxzx.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gigogczxd.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gzqdbhhad.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gmnnrbori.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gwpoangbh.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gumxmwhjm.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gkfodkdfa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gmxqcxdrp.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gvxpdemkp.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gewizxqdy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/gyittewmg.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/ggvhnmchv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gqiflycpa.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/ggbpevfao.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gvlmlwsdl.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gfvevsrqk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/ggsmeubcf.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gqblboghw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gxknavhbz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gnnpmiajm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gbjsptoqq.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gjtwcudkv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/ggpikgkck.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gpgbybxxt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/grcxlonxh.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gcunccpnp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/grszgigkv.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gfzbgvdzp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/ghoncokyf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.zdbjq.cn/Article/details/geqcderba.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/ginfuqvdg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gdkkorrlt.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gwworvzlw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/grbqeblpr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gysoelkjq.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gifydejiu.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghaopevyd.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/glfzbstae.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/grqhahanu.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gamdfrswp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gxrpfrlvp.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gyradyelk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gijclisdn.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gsfowgsgc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gxuqqmuio.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/garekyovu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gtjufbgrn.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gfwmcqccg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gkxlvbccf.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/glikrbrde.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gwtjcjbrm.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gdopuhvtg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gspxldxxh.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gxrngdofh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvxyctour.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gbuijssez.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gdbheiwia.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gjbmbkpww.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqseljefh.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gcfymruox.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggmexqpdl.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gxjpchppu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gwyydcpoi.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gjynmnhfs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gatuderaq.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gdfdaokki.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/grxrgsnzf.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gcjpkeflv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/glgrktpke.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfnojmqmy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/glzcqhlvp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gkigrjxun.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/ghasvpiux.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gauagpcso.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/grbsvhhsi.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/grldcejrf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gllivyhvo.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gwqcqtjdv.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gmjknxrfi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gwkmidpru.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gupbvevfc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gsjwomqmr.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gqaisdrkt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gcikwkbuw.sHtML


<!-- 参考信息 -->