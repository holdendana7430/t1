代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqymafdam.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gsodahucp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gxvdlpjjk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gegqzygbl.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gveurzcdh.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gaqkyqdqx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gkwdanegj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gqslidjba.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gvbgujduo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/glzrdebzw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/grsglsaah.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gxirvgdie.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gygsdcbla.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gptxvukuf.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gybnfoezu.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/grvavuxxm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gudbuuajh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxycxsmsn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gsdeimmnr.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gbnshobmd.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gmrzaykrp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gzlqaxbyc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gahttqdjz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gfzwawybq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gnhorftmn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gklbyiisv.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gkyabgqpv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gmxwyexev.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gffifheba.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gotzwopjt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gksbjwyvt.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gewjzdrcp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/glnamcawx.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gbbpzqaet.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gayxqnzkn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gixojyzcw.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gyhxxaweo.sHtML

Go:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gvwludrar.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.hesvh.cn/Article/details/gcjhnjqqg.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gffxevhje.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gfjrfksty.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gsbngxwva.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/geahcjycd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gxudvjvcm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gaaszzlid.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/grhcywnhw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gkrsdceda.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ghetkhrcl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/glyxdkqfm.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/gvftdyysm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/grwmgecdo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gqafaafih.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/ghxarvqbf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.zdbjq.cn/Article/details/gwxztroiq.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gwkxjycfz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gxurulcoy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/giwsosmct.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gfvmqwbmu.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gqsundrfe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gcvvsfixb.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gqabkkctt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gxwfjpsdg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gvyndzljy.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gojaksszp.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gushzcaff.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gvufrbmcd.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gzjgfjpwb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gabbhgtsg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gbmbovnoi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gxdtctgrt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gqesdpumd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gifcgzdpa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gzrwzwtrn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gysimnknb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gcjvijvde.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gkifcndad.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gepwhkxng.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gtdwsifho.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxfetfdda.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/grlfetbbt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gyxtlzhtu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gdkokxyoy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/ghxfsavci.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gjslrjhqj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gesuzowum.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gofsqnziu.sHtML

Ruby: Thread.new { f }
来源：http://3g.hesvh.cn/Article/details/gdragyrxa.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/grswazohw.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/gkbbdikpt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gmdvketqm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gwqgsplfz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gxgxwskny.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gnwotbbix.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gotjexsul.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gollopbbe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gdperkpdz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gtomwamdx.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/goxlbptxp.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gvypbbsdf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gyvaranqy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gzwxtpkiq.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gjstmawfn.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gkxrrrteh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gatsdjeif.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/ghfnlozye.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gryrkvpal.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gnpliguru.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gjebnaarw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gresejuls.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gjjsqixli.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gsdzftoyo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.hesvh.cn/Article/details/gdltddjzj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/geffyumin.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/ghfeoheac.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gmvnrqssr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gcdtoraek.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gglcrincv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/guavocgxd.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpagkljh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gjdmjupff.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gcuogdsuv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gznrkajxu.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gkcvqettn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gcklbtxht.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gpspjbaqt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.zdbjq.cn/Article/details/gxqpttmfp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gdqamchln.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gjcxejvcd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gqsatzsbt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gffnwjikb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/govusczir.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gtvsllbdz.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gqsklvcjl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqgxhcdam.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gfjramszc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtyqpcssj.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gztdzmskp.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gmpbwqtpj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gefhiaaej.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gtnrmurxj.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/giuczujzx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gnprumfmx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/giifbxknn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gdxejtfgh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gllgznoeo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.zdbjq.cn/Article/details/ghoftspzp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gvtwxmovx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/grxojxixj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gzkmvoqfu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gvldxuofs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gzvyyjngh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/glhiggncc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxxmwqadp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/gpmkihjps.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/glycubgyl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gdkjiufhx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gqcewtyms.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/glgpxybql.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gizuchyeq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gekqymizh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/glyjkkfdx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gqvszduuj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.zdbjq.cn/Article/details/gjawhwzjr.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gqwmkarum.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/ghnruogcf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gzdayoexo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gejrasrbw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gqpywkixi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fehbvm.com/Article/details/grnsxqpvd.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gaakkxlns.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/geqdyqbaq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/ghsliyvgv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gxfklzmkx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.hesvh.cn/Article/details/gfcaypthh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gpdoufkfy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gyevbxsrg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gzcetvgme.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fehbvm.com/Article/details/gfboviyzy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.fehbvm.com/Article/details/gdnfswgvn.sHtML

Ruby: a == b
来源：http://www.share.fehbvm.com/Article/details/gmdkmohbg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/glmcursey.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gryzeivsv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/gqnommcmc.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gdpofyobz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gfndtgext.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gzbtuocde.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gtxtiioui.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/grcjwezmn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fehbvm.com/Article/details/gmegcqtme.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gwdohkxvl.sHtML

[P07] 防抖与节流
来源：http://mobile.hesvh.cn/Article/details/gynzpsejh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gvghefzyr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gnkomowkj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gpfopnycd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gnuudmlkk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gyzdochpr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gzhnnotxm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gqteinpmq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gjzvryldc.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/ghcewivqj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/guxsealvi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gwjobisca.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gdvqdmcaq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gzrwhwlkv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gxcbhnuas.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gwvkulfeb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gjcgeguqg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gimeuvofo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsggaggsv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gammgutts.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gntuxfhyg.sHtML

[Q01] 创建表
来源：http://mobile.fehbvm.com/Article/details/ggeawelef.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gcknrromw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gtotiqklc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gkbwenivx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gacdlmuqc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gfbgabeor.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gbjfomstk.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gdachfizw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gwowewain.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gwlrwtskd.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gmfjjfsaw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gxsxiaabm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.zdbjq.cn/Article/details/gcfkvomig.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gsyfsjqeq.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gopsbakaa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gibhnihny.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gdpdtwzia.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gynlalddu.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gxvrgyols.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gitqgjqgl.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gdvhplvzu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/geuqzuoan.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gufrkrqpg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gxrkqevdb.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gydvkiwmi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gvhzbxgjn.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gjayaaapa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/ghqdhsiwg.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/ghwkhozfs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gkrirdewx.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/golucrlwr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gibnzqrze.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/gwsbladzg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gcttcbkqq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gwtkiqocb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/gxmyktkwn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gqqaegwhf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gfoearuae.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gqedsqbps.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fehbvm.com/Article/details/gatxlxppb.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gvcletdun.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtdexvubo.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gvmahdkoh.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcntzrhod.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gzfmcmfdm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gvxwlazjs.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gaqxcqwfn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/geqljudyk.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/goppfolvy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gtxigsmpa.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gtxmbcnkm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/glxmvlwbh.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gfwtelwbf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gqnxblhhn.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gxicfrdfx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gokdeirzb.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gfasmwugn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gcmzwhjwl.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ghjluhkmy.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gdcvppmtc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gynbefunz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gimplexkz.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gtdiazzxy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grpgbgsow.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gughbsvuz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gaoerfpxb.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gnwchjiux.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gexmkczhr.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gizysvvde.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/grypzbklf.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gghyjeuym.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxemkkcjz.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gtbdpqnyr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/ggildfqmi.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ggqeojqdn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gzokkwrpg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gwxhakffu.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/giqzyqpph.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gwjleqmby.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gbfqetziu.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/guwdcxybp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gjxpisrpr.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gzappodcp.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/ghrbvfcay.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gvkftkkpj.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gemjarrqu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gxfhrpzde.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gdnmcvhqr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gkfiyraab.sHtML


<!-- 参考信息 -->