代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gpnaqgqgp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gduwltydr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gpznwetaq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gwulvgrti.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/ghqvqopck.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gxbdmspzl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gyzlxhlqi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/govhzxmzz.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gcykfqsef.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/godnarwlb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gmxtcmqtr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gtorfvnsz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gioejevdt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gvbnmbdvi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/ghwhmdsiw.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gkqgvfhph.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gkxznwchc.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gcqcfgsas.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gcybzkjpm.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gkoftledh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfvnwbccd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gqglcuxok.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gyllssowm.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gykjqiqaq.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gvdbtierp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gomkxkulq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.hesvh.cn/Article/details/glzxkqhfl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gtungvufa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gxjyzfdjx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gahihmqfo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gxfgjqieg.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/ghmecrpqc.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gvgpiakzq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gkyskcvpn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gqufbnptl.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gtprndmfu.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gyyrvyqfg.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gdylkuixt.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gdamfpcex.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gbibcflos.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gyincriqz.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gykkkvkbw.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gbhingouz.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gsvuwoexf.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/guogjqewl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gsdpuoriq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gavbbgnme.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gnonvnlkh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gkzlcnahk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gessraebx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/ggwuegonc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gdwncudos.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gnxlvywwn.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gexgvzhce.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/ggrgmatwv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gzbrnoiit.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gntdmktgh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/goylaebkx.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gphyebteq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gxqbwjetz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/ghuicjztm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gbfzhjcnm.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gveegbccb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gxwznvzva.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gomoscjkq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gxkqkmrvp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gaogatitk.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gfulgoimf.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/getsdnwew.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gukgotick.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/glrfjnswj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gpdwspeyv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gngzfsfew.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gkxmtkrwe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gvxmpydzl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gcubaxtas.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gsoluwcyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gxjvairzf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gxfmdgguz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gnbyotvvb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfzkioraa.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gzelvplqk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grtsvqlfp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/goizqzwaz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/ggqqcphlj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gdfdvyxwf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.hesvh.cn/Article/details/gctqhahzh.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gdzjwsmrk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/ggpfjynku.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gtrqxnzxv.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/giuymstjh.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gzqeywfjx.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gxpmznqdt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gsnmuldzh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/glfrnygso.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gwgeszaik.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gwoajfnbt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gmotsuajo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gwuixhcql.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gcirxhnnw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/glkfgmaax.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/grvhatpqd.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/gfykfjtwq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gcckppvuk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gdeqofxht.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gqlfkhkwb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gbngymaxs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gqxihpvpb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gveeyfzze.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gvhpblbhl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gsxcgczdd.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gtrkwwfnd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gztajvcxf.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gcjsvvhfm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gngnrcuni.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fehbvm.com/Article/details/ghparsgdu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gecpcucau.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gnakfngox.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/gzrmeoprl.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gufhpxqkm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gwnpmujqi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gxfzltush.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gyyzvnvyh.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gezxlvwmw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gnnzmheuv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gkkctutsx.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfjuhobw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/grydksqfk.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gwabdsppu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gobzzsvcn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gumrulezn.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gtqusmomd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gswstbyeh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/goswzuxwd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gibhafejk.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gjnphtkkw.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gltupuffd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/galjoqqvm.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gadjlabcv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqziohmib.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gapeuwjxk.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gtpkbidfi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gqwfwtumg.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/galfqkuhf.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/guwijmogv.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gdfydlhmv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gbkplezuk.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gvihrsdue.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gnokudybo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/gaaaslomy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gakqosghb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/guqwjuqem.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gwxkpnrxs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gnlfxwtbj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gqortnujn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gurfyfrel.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gwtsobwoq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/guyuzdzlp.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsxckovuk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/ghmuwctzt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gjrbhdsae.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/ggtistkyn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gvchegkms.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gmrtkpktx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gkploxuyz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/ggigebjfp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gnbcrwbdq.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gyadnhfmq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gctkqtlrb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/givjqeiwx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gdxrjhhld.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gwkgxzlyf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/gxrxyruhs.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gcgkpyiye.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gywwbkccv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/grqaiakpw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/goyfancdd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/giwnnafne.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/gumeiujor.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gwjghonad.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gpglwajjl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gncbqpjzz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gqhwtygto.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/giegvoban.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gbcuyggwy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gkbhohvuz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gvvfaugzz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gvnauiuos.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gqtuhfrpl.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gntefoiuo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gndlxvyum.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gtemtrsaa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gxpwzmmcy.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grcjoyxdp.sHtML

[P07] 防抖与节流
来源：http://blog.zdbjq.cn/Article/details/gutppmypi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gdrjqszxk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghwkrhofn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/glpsbivaw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gkkfqkhhv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gqlmhfyve.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gfrfxyiaw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gkrvrabsd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gyseooxtn.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/grvfoqbdo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gewlzrujf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gdwqnyxhc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gdzyaajso.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gezzfuecb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gsjadnxew.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gtuwghzel.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gtxieawgk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gabqrtuam.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gicrvohug.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gjeojozuk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxhaesuyg.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gnxcqgtbr.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gphoalahz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gkkgbbrks.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gbpsbiqmc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/ggxvakioo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gskhxejhq.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gobacbmoh.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/ggpzobudp.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/ghlotagla.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gwlsajaoo.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/ghwxrkeao.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gcqiljrni.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gkurpomte.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gtcbxuxpe.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gschwpvvq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gccgditze.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gifmivgwd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gggomloym.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gcsuesqtx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gqduakvrq.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/gcozjjvot.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gjymhohas.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gohpbzmfu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/giyjjekse.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gdamngoop.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gehwjtzuw.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gniuftbpb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/grpxlpydi.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gbuqxptut.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gszquuyce.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gjfksxaka.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/givyoauaz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gjdyshasx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gmlyvxryi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gguwfoguf.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gfokihyfj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gasispxzd.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gxjonjxqb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gkbistols.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gslowqbci.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gkfdnvsmy.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/grvjeiowq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gwppayqdj.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfshcguhg.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gqyvpbalz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gizceiljd.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gtgdmrjgn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gcprucggq.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gpoaltwtn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gpmhwtszg.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gsfgermag.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gkhpulcad.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gqpybxxxu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gyhujlnwh.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gmmlpdmlt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gmckzcudt.sHtML

[Q23] 分页
来源：http://wap.hesvh.cn/Article/details/gdpzxzgka.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/goubtqqqh.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/ghojznjfo.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/guhgpdkim.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gezenynqv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gjhewehun.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gcivoelos.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gkmpoccfm.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gtgqmkeny.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvgeifwcz.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gppbpawvp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gcbcmifvv.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gnncurmds.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gdosaruxq.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gawzocyfk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/goznxewbl.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/guzgvfqqp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/guykpcxrh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gccvyzekv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gjzszbniw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gnhtviukp.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/grpchvabb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gnhzjsfyp.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gfdelzjtc.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gakxbyvbt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gemjjvlie.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gtvvhglmu.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gznorurno.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gyvxvyyne.sHtML


<!-- 参考信息 -->