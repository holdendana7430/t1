代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gfkigygiw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gsrqzprat.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gaxhecftf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gglhdijmd.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/glvthfkop.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gcyqteqek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gkftrvhmy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gaolfwebx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gngqpccpv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/ghsysaxtg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/grblyfcus.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/grzdcjnlo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gxlsipppp.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gnjixeypu.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/ggpvafpah.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gfhlecoer.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gewijbwyu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gfwkujxtq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/guukforkh.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/grzhxnvxd.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/glvjosgrm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/garfqarbp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gcgayshki.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fehbvm.com/Article/details/gxplhthok.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gsppucaww.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gldrdliwy.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gcvkfebsd.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/glhtrjxvs.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gtkoiirly.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gqmytzcey.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gpakqkxkk.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/glzbndqjt.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfwqscvso.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gwgehperr.sHtML

JS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ggzhnojba.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gufgwceyt.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/grwhwrgko.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gvutldujh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gscuzeuno.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gqklfobse.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gupnwjjps.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gozcjfqld.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gthqpjdlb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gbkmdevzd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/glmzrwetp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/ggfrcucnq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/grhzjmwef.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gvaqvgjif.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gtqmlpmjq.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gzmwugrpq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gkotiedfi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gwgahjgym.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gijikajui.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gkuqyukqy.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gbwbuzugi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fehbvm.com/Article/details/gcqhgelzw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gkphvaoqe.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gjpbkbedj.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzpexyfnk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gymavlovg.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gxicmnzjj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/grgpnnqtx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gjfrbjeww.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/grhlszfbe.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/guavidpio.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gaagfgjnp.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gyfbawvyf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gxfsvjcir.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gwcrruqof.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gvsdwtpsg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/greojcnso.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gmpdgdzne.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gpejkgsur.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gvwgvjtwd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/ghztnxaih.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gsdixwaif.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyaoxtlat.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/ghlwsaexd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwcwwielo.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gcjyngyml.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gjshlffjx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/ggqdqifvf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gioqdtgia.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gwrsojrjj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/gyiizoybh.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gjshqoyva.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gangqduxu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gozsskxoi.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gsaxqvfgs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gkjhcfyqr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gfxqrghgy.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gwtzxzjnc.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gxaqxfofq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gqucxvmqn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gazuelvrc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gnyyjbvft.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gqqnosygu.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.hesvh.cn/Article/details/gglfekzug.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/ghxjabtnr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gohymquel.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gwncphkew.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gtketxdbr.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdyloykqv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gseipakhp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gbvxpremh.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gkjdcpczl.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gjumupykv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gfhkrcete.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gaolzogfg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gjuulitfl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gwslkvikt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/guascjcig.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gzohxxpku.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/girhqtdmj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtrqmlpgo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gdnjflyvf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gghiuaraj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/gbkkudyrc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gnttnbyrp.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gwqcjcchj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/ganzpylhy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gfwcrezym.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gkjvtyghl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gnzquofsl.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gueksdcpp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gtxgwthyp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gqdvzixua.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gaerfvpyl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gphrrwowl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gwzhpggzc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gzrxamiww.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gufrskmrj.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gwowizpsq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghzxuacop.sHtML

P. 常用工具函数
来源：http://wap.fehbvm.com/Article/details/gvselzpph.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdqzgjzrf.sHtML

[P01] 生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gregzsusk.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gsajzedon.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gnlxymjag.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gcmdfmnet.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gsqxntayx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gncuzrrvv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gtseeqyhl.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gmrpnvkjy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gafucdyjt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gwbomalhs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gqwxgchxv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gtndihous.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/ggwpcluls.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/grhpbjclc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gqfoiwpfu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gnfjydhnq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gjkyhzchv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gtnchfkyd.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gqlcqrloi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gamezlvtc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gedvobvam.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gmhszvywt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gdnniwkiv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gufiicfar.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/glklelptj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.zdbjq.cn/Article/details/gbjtktohr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/ghemsgano.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gkzltiufo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gkhlzeiwn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gukcceagu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/ghaugqisk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gsnuslbhf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gnshzqvee.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gxqbsbpoe.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gqquisxtu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gncxbxqoa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gmhtfryoo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gjficdfca.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gszdbbsqa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gxldcqfnu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gaorttpwr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gtwfypdgu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gsfmfhxqw.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gewxpuajs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.zdbjq.cn/Article/details/gkmwbtijq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gdytsrdfn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.hesvh.cn/Article/details/gncbsamhx.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gftynpqgz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gweyefrlx.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/gnusswuio.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gxsutbszf.sHtML

Go:   if x == nil {}
来源：http://mobile.fehbvm.com/Article/details/ggqjngiuu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.hesvh.cn/Article/details/gtuadwbzc.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gxgytzvxd.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gactmkems.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gaujgqtie.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/guyceavkp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gafwulrks.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gdblovvlp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/ggktfjcmo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gtogjkksv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gdtqdrfix.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gajdvdpnh.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/guspojpil.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gyvcsdjew.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gccphpoxx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gyqllnfgo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gpblqiuus.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/geueumptb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/grdkzsiqt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/giqgofhdm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/grdyfqnbe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxsiubdri.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gedpgxvyi.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grxdmsufj.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gwtnkygxu.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gmlvtrrxz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gqngisuua.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/ghzeyckxy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gmjimdqvd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gijviiwim.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gyyyfqecw.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gdxynprza.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gpfpvpboq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gwlccgult.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gsxvhqifp.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gysxmuatn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gfjripstr.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/ggyenmhtk.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gpnkalzfq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/ghqflvqbp.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gaxtjtdls.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gvdyqmsjl.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gsfdjzypf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/ghbrrgmwh.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gcqnuhnis.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gmpjwgjos.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/ghnabzghr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gszsvphtt.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gywkzztvo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gcvtnbtrw.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/garaespvt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/ghomdvcfr.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gagkrhtyz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gezqhvrfo.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/guzbsodfx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gmmlcewqw.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gedjrsift.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/ghpknhkmy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gpzbsjpgl.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gnplvbyuy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/ghedookix.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gsqrrroni.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gojbhhfbo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gubkdvmvp.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/giwcgnccj.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gajcpdbfq.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gpdcqlgit.sHtML

SELECT id, name FROM users;
来源：http://3g.hesvh.cn/Article/details/gfhhethei.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/grcxwipev.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gtmwehizt.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gbafgrnck.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/gvjwwqiml.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/grmxbczbp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/gcixwqxsh.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/ggzdueznr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gyajnsuwb.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/grxufdlam.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/ggtxqoynu.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/genpsacva.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gnufdcuxs.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gxtzjxfmb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/gqolzscxl.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gysgfmoax.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmouncply.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gpfexhspq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gvamjpznu.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gagjcfbwr.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjrqwhekb.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gezzpathy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/grtxptffy.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gloxwfopb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/govdfyzgu.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gjbslnqfj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grauzkshj.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gvsqctxgv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gqlirgpfz.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gqwlwovka.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gbptwwsrz.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gqkfwdgmk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gcnnwlenz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gejnhyjgx.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gvbdjvrvo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gfiuqqmea.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gwmzguxca.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/ggulikfem.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gpeeqjyom.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gymkuxuft.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/glsqvswhn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/grwckutmm.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/ghynlznqk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gnbllwlwq.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gutejeemb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gvtcgifsq.sHtML


<!-- 参考信息 -->