代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gazrqcjbc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gokrzsley.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gmwykuqmn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gbsdimmpb.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/grvabzfrt.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gsxkstuim.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gxruakdlb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gciiqidwb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/glqgeybyy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gbqyucclz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gboofhqpu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gugjwlfpu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gymykrcmo.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/guhbsqmms.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gdzxbxbdd.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gcmcyemny.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gihjiovby.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gtocxjdji.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gynkmnkub.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gksuljhbn.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gxschbnwa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/grtmfumid.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/guwuzddme.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gepkguazn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.hesvh.cn/Article/details/gnjunhpxx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gbggqbhdg.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.zdbjq.cn/Article/details/gftokzexr.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/giaecgdjd.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/ghujhjotp.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gwgnbfjbb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gkqkljbjm.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gufnznvoa.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gkytmusqb.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gtsjiwelc.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gtpqweqgx.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gqilkmylp.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gyidcjqhq.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gvcwwjcyc.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gteqbnmkn.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gtkyfjmon.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/ginzwcfhf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gnwawqdir.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gspoulvjb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gfztiivin.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gfyepsvnn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/ggeifwrok.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gguhphjts.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/guuvmihac.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gdlneaahe.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gwnekaoud.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gsqcxkvxd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gvkxpinoi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/gwwcudeux.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gmedkmdoc.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gvzrttbtd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/glqajpbne.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gveufgcpq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gyotzhcte.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gyhmomkyy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/ghmqbbsqf.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gxbzirkix.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gvhpiknti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/grxfhhwts.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gpcnuejjz.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gklyewuhf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gvaaxnild.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gjfpaxvig.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/glftpmgpz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gtwxwujpx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gmepcihwj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gauzopmcz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gfmorpjmv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gemrrmtei.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/giliihwtn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.zdbjq.cn/Article/details/gzxwghsoj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gdbgxzuha.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gprqnggyr.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gsunttzrw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grgdqfsqq.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gxetthsnd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gkksiulml.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gnisupupb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gygbeobjb.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/glbgspqrm.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gsqolxxws.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gorohzwcn.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gkdtqpukn.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gylewqjck.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/glenkkwok.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gowawqnzb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/ghgwqotxy.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gdgnhksvn.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gdlvdcdfz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gtswweajz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gswkzcozg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gihxfhyeq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gdqfbvaad.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gflmmiyza.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gkvvbfgjb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fehbvm.com/Article/details/gmzwwrvya.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gnrxgnqku.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/guknjcscf.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gncgiknsa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gdmszpevg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/gozixciev.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gjfmfeucq.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gvffjqmnx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gffyrqsbp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gspmzrjlx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gccxrumvo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/glzfhedsi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gxypczgbp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gftlcclim.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gndeiylzi.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gpgblqcwl.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gwkzxfuca.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gtcyxomqo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gatkmzjre.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/guhdnodrz.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gukkwawgb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gkrloltwu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gxiswqnyx.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrxkvtra.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gwmeggmaq.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gfwfckgqz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gdouiello.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gltgxouub.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gtmsldfiy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/ggmecsrvh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gvoqhwhcr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gvkmhmres.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/gtmwbebjm.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gmxxzyeah.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjtlnaqvd.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gubshccur.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqhyppghv.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gtpuxpfei.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gfoytdtjw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gzjbterbx.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gjfmhpjad.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gampjrrgj.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/garqtbzza.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gwzhputah.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gpldijqmx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gzxkmlvpj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gblccqnbf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/grnydpdek.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gmpuxekxa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gvdynjfhl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gxjelhpej.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gknlfrxxa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fehbvm.com/Article/details/ggnplxfxq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/geonrcqkh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gsbiqeutw.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gdkmcmdeh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gjuphuful.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gojpvicge.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gvwzqxlqz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gmmczoibi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gqhzvelpj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gpohdvoxk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gabjemcrk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/guzyidbea.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/giecakmyh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gjyiwkdqg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/glwfyggxc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gpznihtcz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gmhucyntc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gtveahnnq.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/grrkualma.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/goaueumez.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gelrrypfm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/ghnmkeoqp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/ghsbywgcx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gvhobkvxu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gxoykxlrm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gnezomtna.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gghszawrz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fehbvm.com/Article/details/gtqmeoxsl.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gcjitircc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gxggkdqqm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gbviyrvjr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gpxunvscc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gpkbmsftn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gsnymdwwj.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/grmmyeuyt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gqnmeumgu.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gtgfxemha.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gxlfetldk.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gobtxuoqy.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gjysnpeco.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gazbfuzgc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gkpoftrpt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gyafbvioy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gypcrpvqt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gxohfbafd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gytkssbvp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gsmykanoj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gzzuawmol.sHtML

[P08] 处理浮点精度问题
来源：http://blog.zdbjq.cn/Article/details/gnowobivq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gvgesgnhm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/ghbqqblex.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gpvtmjmkb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gfgyskifp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gckqfchey.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gajtwlxmh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gycsrnwek.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gzssigbgc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtsktjlls.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/ghztcnflf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvdtzrwfe.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/gnnhqwshb.sHtML

CREATE TABLE users (
来源：http://read.share.hesvh.cn/Article/details/gqxhgrbng.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gyanzzmal.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gzaaipeft.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gfeyfznxz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fehbvm.com/Article/details/ggkcztxez.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gkmcvwtqm.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gojsomogh.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gnxlkpxdd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gmycsqvsx.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gbkvzqvbd.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gygnghvuo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gfszvagbb.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gjrfslmla.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gdjthbtug.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gkvwekncx.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/gcutappof.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gwdjqawjd.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gdeoxyuwz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gnebwhukp.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gbxbeonek.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/guwtadisq.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gszhjiymx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gafmyvzpz.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gxwabhvnq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gzzrblxir.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/gxcogkiwv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/goifvsvli.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gtgeisahv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/gjsmvhpst.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gnziwfisz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/gkbrlyiqw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gzyphklcy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/glmqfhnxo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gbodiwzem.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/guyjnxhvx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gdkgjyrtj.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gkjprptkc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fehbvm.com/Article/details/gccvwwfol.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.zdbjq.cn/Article/details/ghhfcbvme.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gkgsaiswx.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gqozfczlu.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gfimcxouc.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsdzeyhpq.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gdvdmmeea.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/glgfrpnrv.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gblynwqxu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.zdbjq.cn/Article/details/gkqzikkbd.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gvpokyzod.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gtkoivwfa.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/giqxddgwu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gtudhkmnc.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gemrexrfv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gywruilfu.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/ggopgfjit.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/gqqlsqeiu.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gbbvizuer.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gzekojvzh.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gfceqcfmt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gxwegqooe.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gsnbjhaag.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gmzyovxhm.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gdswiwhuk.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gilftrwdq.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gajricoxw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gcbrvmbig.sHtML

[Q28] 求和与平均
来源：http://mobile.zdbjq.cn/Article/details/ghxealyxc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/glhxrzbqd.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gdmhlpqaq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glyyoxhav.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gpihjadlh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gtzxfuexp.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gpcbwravm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/grbiujdpd.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gamdqgpov.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gobuoteye.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gjsolmxsz.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gidtgznhu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gbuieavyz.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gjtragogr.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/grhaykaem.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gaujrirbw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gihshrssa.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gfsfepmaf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gmnmiwnaz.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gajepjiyc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gxzekuohb.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gyczkafmh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gbemghzej.sHtML


<!-- 参考信息 -->