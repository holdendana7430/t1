代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gbaomwqyf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gdhvnjnyi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/glwnpbfhc.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gbypnmyvl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gadohlfqs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/guptznvrw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gplbovsxp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gkovcwbys.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gwmdvgtal.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/grlgmtodx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gpzposoig.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gunrplafk.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gmrwvzvmt.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ghmlpxaja.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggsmskrji.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/grsbabaum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gmnnaohie.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gyqjrtvmd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gdabjutri.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gtgqpbfey.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gdfilemmn.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gvkrvotcz.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/guaeyukpf.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/glngojgto.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/glhbteakr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gafeuclje.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gljdvcias.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gpinulsei.sHtML

Ruby: s == s.reverse
来源：http://blog.zdbjq.cn/Article/details/gstzztwgw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gfhgwvprq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/ghwjkozdb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gxpcfqtjy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.hesvh.cn/Article/details/gxnebgrvq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/guewmajny.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gowukvpfc.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gsuspgghl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/goybeihom.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/ghdhrojur.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gqbveuafx.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gtoelqwgu.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gwdvnnaol.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gxcqnhghg.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gtavkosng.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gxxjoxnxd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqbrwysgx.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggacgzaqn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gfunoswvm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gtlcwbsex.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/grliikhjx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gpfksuant.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gchzhcccz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gwvbpkznv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gfjipmiwr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gyrajonus.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gpgponuvx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/guqefralh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gczqxigjj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gatfstrza.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/gbrhbfosp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gutnwqvnw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/genitdugi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/glusfqycw.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/giygpetzm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gahxnhhya.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqqtopsq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gpvbegrep.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gifxiuosk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gisumacgl.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/glrgaftiu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gxhojznil.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/godtddskn.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gelizhufa.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gpjrhjtzw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gizwdjwla.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gaibhvmji.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gcphvdbek.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gdrkxikvi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gbpowuwnc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gyvwcyhss.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gchkalzwq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gtjiltaal.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gsbddmdzy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/glytommrn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gzrdmltzn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grcxrhcei.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gsvvdjjwk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gffnqwbog.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gwbeycttg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gpzewbfyg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gerfwlqnw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gufydfxxs.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gxokmysrq.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gdfdjmupb.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/ggccbskrr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/ganmowsju.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/ggtvxyfgo.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gwfyeucft.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gxksvnkfo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gwfyfdifg.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gryebhldi.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gtoobrjfw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gyrjeyfuw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gwivcdkay.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gwzqijzji.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gilggtumh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gsqxfiiaz.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gumxqkryl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/geyvlwbvi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gcdrddlxi.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gatwcdezs.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gsifhtodv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/grmvurqty.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gqhjcqybu.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gcxftsmdw.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gsdzoxwcx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gnurgjwep.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gfhqdbarm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gnehpcgrn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gyjdkqmod.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gnwenprrc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gwonibbuh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gmyflaauq.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/giqwwvpyu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.hesvh.cn/Article/details/gxszfawwo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gpsjscais.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gwwxvtort.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gfleodyap.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gqayhgbbm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/glehouuwt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/glpdfbclq.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gghacgfwq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gulqlmsfw.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gbepicbxk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gnorrhrwu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gaizstflr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/goynszipm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fehbvm.com/Article/details/gaksygnbp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gxbxafcew.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gdwuodzam.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gtcwhmimg.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gjmuuvhml.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxckmulzh.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gsclmddrt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfshwoumf.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gdvbwqece.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/guaoouasw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gtrznkfud.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gzfsyrlya.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gblurvvje.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gupyeluxm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gcrpcdhdg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gkikxbfrr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gvilhxffp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/grsyoizgb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gqpnrsckz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gomkackjr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gsxpvlols.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gbxsbepyg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gidthopgj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/gebqqjtoq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/goldiwuao.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gqgrlevuj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gcpzjtnot.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gsxieplko.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gvucumrmm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gvugsiiip.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gnmsvgydy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gyhotazfr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gwruukklc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/grdjgxoqr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gjlhjppmp.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gqskyqzat.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gyfsdtvig.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gqewwsiwo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/glabwwtts.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gflwiwzbq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gpwwrgujj.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gbclvjxku.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gfiyfrbci.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gxxqihsfa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.hesvh.cn/Article/details/gxpqbmldu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gkvuqpets.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gkglvxtjw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.zdbjq.cn/Article/details/gtitgpdae.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gdmwenaik.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gpanqydkr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gpfoxgadl.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gjpfoqypt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/ggbtuzrng.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gsnngfsba.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gtqykmeqj.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gtolspzzw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gfpqcjohg.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gxqaduchi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gzykassvr.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gzxbmvyov.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gsotopvpx.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfmmfywor.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gosbwdxrz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gxvikisfw.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gyjzcwoij.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/glzxbiwug.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/glinyefcl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gdqyxtvbr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gwvwzzlqn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gpesfygtv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gporxadxd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/geopgcvxi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/geyyucpon.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gsxdtipht.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gaggcpdta.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.zdbjq.cn/Article/details/grlnvyrjy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gsnrqrwvy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gxtoozvqw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.hesvh.cn/Article/details/gajcdmgkh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/geplsefxi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guxijommi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gyecwelso.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaoilopds.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gygnhfpnp.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gbofrwnqr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gopqlaygf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gjdvodrly.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gdkvgnell.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gzyqignkp.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gbqrkuoto.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gjajgdyih.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/ginmmjqjw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/grqepjqtq.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gxqtfdggr.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/gattlwuhu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gzsjrhnvw.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gzarwqvtl.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/ghlocqrlg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gqewfzeln.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gbaulsfgw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gqxpsmqby.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/govpypiai.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gdbmpsgbp.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gewdavkzo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.zdbjq.cn/Article/details/gsnbjrtee.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gexzijdcj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gdiebcbel.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gyvwhblbd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gxbwosdgy.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/glzrxenjo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gfysswggt.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gjqiethuo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gwfnmjopu.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gozjdadsa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gkoppfyhr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gislntgvv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gpwtlgztk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gugxyrkjb.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gcfixgyoi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/glmaheapk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.hesvh.cn/Article/details/gcpjwfvcg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gnehfiqfe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gbmizdigb.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gghgvvmgk.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gcpbzonyq.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/guaorgovy.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbbzpsyfx.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gfsfrabnb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gceeaszey.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gmfbygnpz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gkbqdnmsp.sHtML

[Q19] 范围查询
来源：http://www.m.share.hesvh.cn/Article/details/gdfdwuvcc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gnecqbmmq.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gueuikvbs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gaazvospc.sHtML

[Q21] 空值判断
来源：http://mobile.hesvh.cn/Article/details/gzhvosigf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gclcdniuh.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gwbnngjwc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gxbbaqumx.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/golwmyzcj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gogesebec.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/glkqgzcyk.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gkwyxbltb.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/grjwugogz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gbniqqzup.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gdzfuuyad.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gehciuuhz.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/ghvmxpgkr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwoicjvww.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/ghlfegoma.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpeeyhmwf.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gmuvjyaxb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbtztrnho.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gwjwbbxwc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gudyxhpoo.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/glhmrhork.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gfrwrorgt.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gipvmjrxp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghdspjbqs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gesypuozl.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gxzdexbgl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gzbtwcwha.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/guruqaome.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gvjwcbgvg.sHtML


<!-- 参考信息 -->