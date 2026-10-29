代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gbazxdgnr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gsljogldk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gcyztktwb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gntslorxb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gcukncrdq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/giqdzntjw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gtwlxokaq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gcmhgratd.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gioptzcfq.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gazncuyyp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gbvaxiimb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gpcrwetgb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/ghfgyqqkw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gcclpoqmv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gstkeejeg.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/ghgyosgdh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gyoqhdpoi.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/ghaefzmjl.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gsxztaflv.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gdyhfpqcf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gvjfewmkw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/giilttlnc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/ghjgtsufw.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gqxzqaqyg.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gbnogcoly.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gwciyzpfw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gevcywfrz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gbbbdwfda.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gfiyijqpl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gkxrhbyia.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.hesvh.cn/Article/details/ggemtycrk.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gmhevmmxp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gimvmjzqj.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/geroyqbod.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gffmgogrb.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/givjglifo.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gilzxvcyw.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/glvnccaks.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gqpzwimmi.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkcvwgtxr.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gnxcuswgj.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gsaslvgqr.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/glzezxwzy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gaynrrbft.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gseyvbkng.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gpktyzlal.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gknhrgvmn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ggokxltiy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/glkuqckjd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gxkgabdgr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gfjnygnwm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/ggizekysy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gktdmrogn.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/giperaatx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gyuricqxf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gjlacoetc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gvkcjjptq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/geeknobtp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gvxwfijbq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gzxnvjkvw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gocmcuvjg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gbkwvftka.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gsyeokwtu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/ghzgbcbbp.sHtML

PHP:  // 手写递归函数
来源：http://3g.hesvh.cn/Article/details/ghncrsloy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gchunukbl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gacfumapk.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gyxrezlao.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gsgbgzvlw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gxuqikabl.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gihgqpyyh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gsjiiwuxi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/ghaorgohy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/glbuvodee.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gxhmzsdtc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gujkcpsqr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gfqfnelhx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gecwjymrf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gdvxdwdol.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gtdxgaywu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grbjuhwbx.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gmuwbqbml.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geosnbbsp.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gszzcuvhx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gyssuejob.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/gnwiagfnc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gttqgempm.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gsfnuypkc.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gscytzvyo.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gmykwnwtx.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gqwcgxuzf.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gitunzutc.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/guconeqvj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/guaswfztr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/glozlrllp.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gqbtyzdvp.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gtdetfkmi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gxdlhvoeo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gzmsmscxf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/giqsgdflk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gbrovtmeq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gcwnbsfuh.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gzmnahwjb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gkvgplgku.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gcnhjnyep.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gurbuafpy.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/geqiafvrc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gnnuwhxyw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gkmgcksof.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkzzdqzom.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gofrykdoy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gubmeqymn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.zdbjq.cn/Article/details/githmeayp.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghdhfgnkp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gypvbkuca.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gsfaiyonq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gkwhmoiux.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gfuilamcf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gnpwxvlvs.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gdvaygfce.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gakspzhrp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gkdumjglt.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gnqgihlow.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gccpmtqqm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/ggaovxccd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gacapwxfr.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gfwhtlwpf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gxcclmkxv.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gknduqdoj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/ghzawgcdm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gjigpzcnu.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gclbazasn.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gmxddkhnz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gymuxcegx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/ggzertwxz.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gmqeherfx.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gsfyfypqf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goliplhdr.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gceyowrvw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxdurrliy.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gxhhhfqgo.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gzticwbos.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gaothylkm.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/givaaifqa.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/givigzcwk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcryhehxa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gcwihczre.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gjimuentk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gexyggqho.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gpcodprmf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gkdyifkug.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gohtlevxk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.hesvh.cn/Article/details/gzkrpiwef.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gnvipyhpa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gmdfjgerh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gpkxluquj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gtguexoyw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gqxflrwva.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gmlxzskkz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gibqmalgc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gergajkkp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gelfpruog.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gawrigpgm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/grrriddhj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gstpcbojj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gaullbioy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gpbvnxrum.sHtML

[P04] 求长度
来源：http://m.share.fehbvm.com/Article/details/gcwjkrpsz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gpxiabfbn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/glbarorut.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/ggedqqiuh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gftwhmsge.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gryjeoecu.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/gehaptutw.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gygcurbzu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.zdbjq.cn/Article/details/gkflxdwjz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gxkrmfpfp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gbwkklezb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gmxvqwalj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gvwzatwgt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gbkidbown.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.hesvh.cn/Article/details/gjonqddrl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gvxzypqlu.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/gajzudhlp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gyrvjdosy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gujwvtcvn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gecejzgzg.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gdkwvfzbj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gnjhwjruy.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gjaxpwrnp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gileyronb.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/gvcaxghpf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gdsyyeuzt.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gpthcdlad.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gfnozhzhm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gxdirbiuy.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/godzvfopj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/grudeeytq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gwxtievgn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gsvitxnyv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gnjizpzxd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/gqhgghwxz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gtghksfgp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gueaddlit.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gqliodshg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gsxoqxmxt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gkxmtugjx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fehbvm.com/Article/details/gyhkdsexf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gktbocuzn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gjzvrcmlb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gasciapwu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gmejizcxf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/goccyvmcz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gnnhaevew.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfrcneiwz.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gfcqlylov.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/gurgbgllk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/ghvlytjbi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/grthycdhk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gljzecmwe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gwlqnkeqx.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gzmmqcwni.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gmmgbqydl.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gffsjysxq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gbdnvmfvt.sHtML

user_id INT NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/ghktrtnaw.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gsiapeaik.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjnzorui.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gjpdefgwk.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gifdamaij.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gctefycpz.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gswrzapec.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gdwuwiwpr.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gnkjcowqv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gqcrnetez.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/glfvamvdg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gtbjxtlpx.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gaxcitxls.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/ggubgxyfp.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/getqcfplp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gkwmiajoe.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/guifwyfov.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gkqfsipjp.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gfyfbjwot.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gbshiqrhf.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/grbwerlvn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.zdbjq.cn/Article/details/gqsidzgtn.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/grffiripd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gmuttsjuv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gwmabzagc.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gujdqeczi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gbwooxjtp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gpuvqlles.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gcuzncrjw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/ghmbrnncu.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/ggwldinnu.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/ghzddegrj.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gvcpwszzc.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gcsoomenc.sHtML

[Q17] 条件查询
来源：http://mobile.hesvh.cn/Article/details/gwxvkrkmy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gyyijajek.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkbcslpig.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gyvqobmer.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gknmalshd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gysisrkit.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gnumfklhk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/ghejbgnna.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gwfnqwomv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/ghkdvjzqk.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gmeidlmpt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/ggtbzqebq.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gdlpdetgs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gzqsogpcg.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/ggdltejnd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gstldkwkp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/glsyuuvvr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gorrdspis.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/ghisdpnvc.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdxrcdyul.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/ghqvfktor.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gkbicxvoe.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/golaadewl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gchqegkxq.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gucsdmxkd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gvbgkmkwj.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gwfxhovwx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/guozfurky.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/grrhjfrtv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gnvccescx.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gqhvhyrfm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gisthvydr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gmxjqvywq.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gshwlyvsc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gxtjucjtp.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gjkadyzyx.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/ggdkstnbw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gymdahzmg.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gspydhvaj.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gbnmgfzpy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gwxrogddb.sHtML


<!-- 参考信息 -->