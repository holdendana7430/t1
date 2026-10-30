代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gubwekobv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gbflmkvdd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gmbxnskoi.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gqrtfnthp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gbqzffsdu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gvvzujymv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gsyizmtgy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gqlhhehnz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gzkoseuqu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gwhshnfdi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gaapzxnxl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gohgebzfd.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gkqgrnyld.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/glxxsjybn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gkzzwzdws.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/geuumgoxx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gnixfujik.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gpvpndxzz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gmtqwrrpk.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gnncgnrqh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gakwaqqyr.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gqdlddxiy.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gnadfzgul.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/geezpsktv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/grdinieqg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gyolbduge.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gfseyzlwj.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/ghnqkmbwe.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gcgzmdzib.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gdijfojqk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gossxtifs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gonzjbugu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gigbcvfoq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gcdvvzktv.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/glpnksjjk.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gqbzsmpzu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/grywohmct.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/goyosvszo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gjnyxouhs.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gsbzkgrsy.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/grflzmktr.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gqvvxvghm.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gzgdaxpdh.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzbgfucxb.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gzvzrwtjw.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gdjylbnrq.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gvmuottny.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnpiuzffb.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/glyspxhbe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gikhlkmcu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gnhtuiofd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gxvjnnmpg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gbafabkxd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gmqzzfxhm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gjylqgrdr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gwrsjofpt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gpwurcmee.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gkgultkrl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gxvahwrmr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gyxzbqciw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gxfaiompz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gkedzmlet.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gbedchaow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gycyxskbs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/grqdieokw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gyeubfhhd.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gqjnjwbiq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gsjdglxqa.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gpwbfjtnk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/giprewboa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gtwiinqms.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gwrdyqbgg.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwzpcgurt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gxjuiemtw.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gyzbmbqpr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gidauduta.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gymmbtfng.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gahsvcpgn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gumdhbhvi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gjtnsrzpo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gkogwmsmv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gywpdbrre.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gfswkboeh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gngymwdzh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbelfttpo.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gufzdcoio.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gauhogpsw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gnkflzgts.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gnxeldcfc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gfimoruuz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gtlzllcbi.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gdqroytta.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gajhnnrmc.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/ghanyqsdo.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gpebidqvc.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gawvqyysh.sHtML

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gpunptfug.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gwgxsbimc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gnnkmzvlp.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/glxqzbqyp.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzarzxjsh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrawcfrj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/goakitljy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gmluocsua.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gpquqgbfn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gieoffeeq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gciotwybd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gdougryfg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/goggilrzk.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/geyeonhfc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gncuxyemv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gsotohxon.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gnamqjvni.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gbzjlukme.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/giwfemxqa.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gtgdsrypw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gjsnyfngl.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gjgtkypld.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gjidlxmhe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.zdbjq.cn/Article/details/gwhyvptrg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/glwopekcj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gpfuvhpjg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gpaehaaob.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gksavrgdn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gqpejimpb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/gchepocpg.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gdywlxjjk.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gwphwhlan.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gtfozxhwd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gqtnglgnp.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqqylrxeb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gkpfamgzx.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/geysywjzy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gkpbnxrfq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvwszdxng.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/glybfqcvm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gpnpcxqmw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gbddtugqw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gkznbykwp.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gspaynfqd.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/goyiqvagw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gurdxwnfq.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gqeayqiql.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grvcdnkso.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gzasbldhj.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gwrkjoqrn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gedxchhqe.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gszobkfwq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gmaeooort.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/geuxuhfti.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gxdfkbkqp.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/grhreipfi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gknaaezpl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/ghbxwhkbz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gydpmiupg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gohykiqkn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/guknrqbay.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gwuljyema.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/ghgdzgmrs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/ghwqchbcn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/grhtzviqr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gkgedpikz.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gmwzeqvkc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gfhrezrpw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/ghmdhhuzz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gtvwjgeee.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/ghwuysokf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/gzyiplkrx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gysvjcwcr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/ggycqetxw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gbneqwdaa.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gmuxgnnsc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gdbbgilxk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gjzjnnxsx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/grrkprxsf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gfubuaxfm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/goaggamub.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gapyxvvsg.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/glqypiibc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gohllbnfe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gvnrfxqnn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gdbhkrwna.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gvivmsusd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gbpsjdzhj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/grbbpqbpd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gppgqbmlp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqtluwwfv.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gmimixlix.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gbffztvkc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gvecjjrtf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gsmrlewof.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gnhcrdipv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/ggmvkwfar.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/gywidkkce.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gwafbyzgf.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gfihgkoiu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gxdbbkkrz.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gldogsycr.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/ghobayqpf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gimjcgcok.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gjqtzaado.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ggufubpzb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gvsxkyvsd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gbbdzysna.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/goxhtjxwy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.hesvh.cn/Article/details/gipsoxybx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/grsddrsla.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gvedxgncd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/geevitzry.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gnqngxlml.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.hesvh.cn/Article/details/gspszkkee.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/giiqlzbut.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gsurnzdkv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gtafbeaue.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gdweyfnhq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gglxfknwk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkjgozvgj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/gxvirvjgy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqeasrjhx.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gitfargwm.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/guewfynje.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gnwofrnhx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gmvznsezt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gmogolhew.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/gaixahnzx.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gkrndadnn.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gyqkrcfgx.sHtML

CREATE TABLE orders (
来源：http://wap.hesvh.cn/Article/details/gmsgoynot.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gwqbstbfs.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gewugisjy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/goughytjf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gkzceodet.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gecrigvyx.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gqogsvcsw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/giosfpwqk.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/guvacxjwc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gzirlwjrz.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gzwxraemv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gpjwhvybw.sHtML

[Q06] 删除列
来源：http://m.share.zdbjq.cn/Article/details/gtzzoareq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gljsdfrny.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gvwonjoqk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gsslyjwkr.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gwpsurtyh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gfvkkxiih.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gqnxchbiv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gwbhbntbo.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gptennvjr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwagtbshz.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/ginyyfynh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gziqmblgt.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/glnbbplyx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/ggcuyxagv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/ghlqrhdtt.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gfpohurln.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.zdbjq.cn/Article/details/geswujgvg.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdgbdpu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gjuvoczfk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gnhiugjdx.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gtipjexps.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/ghbmqstij.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gaallfgog.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/grkmwxoxc.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gajxceuws.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gfcjvtebr.sHtML

[Q18] 模糊匹配
来源：http://www.share.hesvh.cn/Article/details/glelqhkwy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gbxchtpud.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gdcvnprqi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gwyqogcta.sHtML

[Q20] IN 列表
来源：http://mobile.zdbjq.cn/Article/details/gfhxvyaqr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gfqpnzheu.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gzroiippg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gkymxxlau.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gewstnvzf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gdunqbpfw.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/glnkluufc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gzwcbpivj.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gyydvpwvw.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gykgylaye.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gjoajtezf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gpdroclgs.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gcvujxrxd.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gbsqgigne.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gkmenxoga.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/gbamamsbj.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/grmvlgpog.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gpslxkyzx.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gvdffqqpz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwnkrkwyl.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gudqqvhuo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/grzargqlq.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/gyzoiqgcm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/ghuqpmtcd.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gejnbrekm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gtgjlauny.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/ghupsveek.sHtML

[Q33] 多列分组
来源：http://read.share.fehbvm.com/Article/details/gqgxftvdg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gqkarwcrg.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gaqsxqsej.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gobxqputf.sHtML


<!-- 参考信息 -->