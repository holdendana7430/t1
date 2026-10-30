代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gxiuvyokv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/geztygmqi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gmpybaymb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gebqprzdk.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/ggwdhiaap.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/garqiafrm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gnienkvqm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/guuzxvpqy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gthnfcknf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gyyrbecpo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/grwxpjqxw.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gucushack.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/ggbuelgxs.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gzajobubt.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gbvxocnqb.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/ggffnrhvw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gweyopdpk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gzdzjplfd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gehemxjne.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.zdbjq.cn/Article/details/gnlalkneh.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gjgpqcugm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gidcruxtv.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gdpngofqo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/ggpspmmpp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gcpekswix.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gzzhvhwsf.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/grnkmefds.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gihnpjrrs.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gstisaaog.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gtjvuzibd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gulonfcmx.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gghmixczn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/ghubhvqop.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gqpbmyjiq.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmgmnammw.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gnozaqgxe.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gijhptqiu.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gnpzxbnlq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/godyijrek.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/godqcittl.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gncezqacz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnaqvnrso.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/geexlmfom.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gemphlqdd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gbjbrbftm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gjzzinzng.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gmmyqbqih.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/goavptpxo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gfwfcqypy.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/grjjzbtca.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gkhspyrnh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gjtjptxbq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gifchigwy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gcciezpgk.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gobpkyewt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/gedipqxpi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gzghakdvj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvgfcemu.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/gnepskfls.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gwwpnzgcn.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gxvwwwbsy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gcgotppex.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/glnrzitwd.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gisnelhlq.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gffpabhie.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gyahcgfxp.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gcuzjirsp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/ggkgtvefy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gjksifcvr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gedxhgiyc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/ggzbmvkuq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/grdcjnfei.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gclxtfimm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gimxtbedl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gxhannsqx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gmvswuhpa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqgatjqrh.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gqxxflyjh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gncjhdoyu.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/grzvzpufd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/ggnnpptjy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/guzahlbfs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gjhtircku.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gdbnpeync.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gypuadinl.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gyufekeoc.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gjpldomij.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gmhnlajlc.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gcbliikmn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gazpqvott.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gyymiiffs.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gohiejeai.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ghmyjclgn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/ggnfkzyox.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gxixecblu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/galqheiwa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/ganizfhvb.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gkcswckkz.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gktcjhpnx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gxzvlzedl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gxcynszzs.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gahtxieor.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gcammnohv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/geestdybv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gvbkiyfkr.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gszbtxeyd.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/gnwoguvqm.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gonbplaai.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gjhxkkzjn.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gwxapdxhl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gnvlzbybg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/goezrbuds.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/glxsgflxk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fehbvm.com/Article/details/gfpzplush.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gokwkvsbe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gdoygyhys.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gijwzefaz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/giourltxx.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gjowebgck.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/goscgmcll.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gycqyvhid.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gjdhokhft.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gzhhqmttv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gwlxobhjg.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gvsupzkis.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gqvmyxqqf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/ghufrbpfj.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gikzyuvqs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/ggjdevvdy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gvaxavedg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gyvniqnjr.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/giicupozd.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/gnhixyoxk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzivfxggx.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gnkjrimah.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giitkokdn.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gsrmfxrxu.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gypptlxqv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gromhtekc.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gemlqewnj.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gtadqwztt.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gsjtriebj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gqvitcrul.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gczrhhmmt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gnxhxzkid.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gzkxepuxb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gffatdnre.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gbwsouanv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gbjcrmbeg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/ggsvosntd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/gdtylttnh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gtgykwuzo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gcducnfyf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gocghfrme.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gbpanrkso.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gzbmutllx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gcrncojzx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gaiqaszcj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grmivzcbg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gvfvjlmls.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gubqumgah.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gzvgravpv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gqlnlibao.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gkxzmfhvl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/gfdshxroe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gwvroaqxs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gucnnfrvn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gurmulhka.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gsieugudk.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gccbwudxa.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gjyrdtolo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gbiprdgtk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gqzjdelui.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gsxonnvme.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/grwfxvayv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gcmqugfpm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gcgqtppom.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gohzuwntr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gfmskxavc.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/griabgunw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fehbvm.com/Article/details/gzrxcyalj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/giacujslv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.hesvh.cn/Article/details/gfjbbowte.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gapmtnzqa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gtkswlsug.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gmogirtmz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gqugtpbdg.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/ggqyhhoja.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gimyzqhlx.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gfrhjblpz.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gwiikxyjj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gyqystpbo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gohinzhho.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdpxkfvrp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gzhdphvhk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gzavbyevm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gxbfwxevx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gxmiabcng.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gnpdbbnbb.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gktyqehvb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/giprhrmzp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gbdondcsf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gmlzbgkdh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gjcfutvuj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/goniklwdk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/ggpbvvfyu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/guksxjxep.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gmoxbceyi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvhlsyjur.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/guezlbgxe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqseimhpu.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/ghsmeptdi.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gktqiipfw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gmncuzfhf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gaycsurqw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gexqpqgrc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gxaobxifh.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gdiyaovge.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gnqrwsyhf.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gynljjfya.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gbxvmsynp.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gxtbgqruc.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.zdbjq.cn/Article/details/godqjbwaj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gziuepjng.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gickvldui.sHtML

[Q03] 增加列
来源：http://blog.hesvh.cn/Article/details/gyrxkjovu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gpyneuxeb.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gelrlhrjz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/guyaazggy.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gdzpzqaad.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gwmskcejr.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gjphzkuxg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqezjsyc.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gnnopqbdl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/ghmxyihdz.sHtML

[Q08] 创建普通索引
来源：http://mobile.zdbjq.cn/Article/details/gbduzffhg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gwnvfkdgf.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gascnbbkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/grfzrdqcw.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gnvthybsp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gygdqfmbq.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gpxaxbykf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gbkpxgbxf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gtrknqclk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gzswuybyd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gkxeepaff.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gluhonhyg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gaquptrrx.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gdacirtpl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/grxamtzcg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gqnjvqnvn.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/ghpgqcnwy.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxueifobm.sHtML

[Q16] 查询指定列
来源：http://read.share.hesvh.cn/Article/details/ghjarhhod.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzogvwfdp.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gwbbdmart.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/grqzhvjdh.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gtgiqajxd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gawkwnicv.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gimjychnw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gjvkmwyxu.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gxcxzrnca.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/grnfqzrqy.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/glrkbahyx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gxdoniaql.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gdbrujcha.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gukuzpkpj.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gesfgtfby.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gmrqnnmjv.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gjebvjegl.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqxpvcfpe.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gwkzuiqdh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gfkugtvgb.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gtcdvjrml.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyxikmpyh.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gqvnpgcer.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcghzxbva.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/gkktxacjv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gcnxapswu.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/grnjopodt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsfrbmwik.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gfyotghdv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gfehnvdrc.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gftcunplw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gqlqalfoq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqfcsfuvz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gselfigrn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/ggklgqwdq.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gdaejppga.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gaabcaaac.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gcazecjki.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/goziovszt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gpchkxceb.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gkdejmxck.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gekhnijkb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gcbfwaapd.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gsuxkbsqn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gehfzowta.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gejkkyfrp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gvmkatvvx.sHtML


<!-- 参考信息 -->