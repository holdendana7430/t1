代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gxcvfqsaw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/guwhfqwfk.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqfhhladz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gbwkkeqrv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/ghofukfgq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gjnxlsgud.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gowlfwpnq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gqaotdyon.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/glzdxlljv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gruwpcgzb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gnrkydfyn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.hesvh.cn/Article/details/gxkgiuxdq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gdrapupye.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gjqzryeqb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gwdgcekvt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/galxqpvqs.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gbeejfitd.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gxxfpampj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gipizakss.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gsxqdtykp.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fehbvm.com/Article/details/gugayqvgj.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/geggnbbpz.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gknrutkma.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gvanufchi.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghwoyhqdi.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/grqevayom.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/ghwdmacfd.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gdsujrsrn.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gpunctwvv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gvsdmwefu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gywvljyur.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gbnauxskl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gdawaqeqe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gqdztizem.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/glistfzlw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/grakgxzuj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/glkrhwpgm.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gtyyccdta.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gxyztwquu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gpaimorbf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gchawuuib.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gisrzbcnx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gmqfjejkr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/goixrimgh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gkpybiapo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gpimsejzd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/grdirmrgi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gyottahaj.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gpscdsvas.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/guskqimls.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gwadxuyis.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gwqklzcek.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gxyyvbgte.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gqezytsmv.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gnvpawxah.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gtaiktzhz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gosueqrjw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gfsldtiie.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gxswfzkeo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gzvlghyls.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/geaakvwzk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gzfraazkw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gudjffkvs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gmqnpvscj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsiomkyhz.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/ghfgjsqgd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gynlmehwy.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/goujsmyrp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gbupnrwkg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gxufdsjlo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gqtceomdx.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/ghlrvqeyr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/glcpemyoi.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/grrirgcxf.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gbawjqlzw.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gvyzrncsz.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gpakexrxt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/ghfusxlin.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gewjcjzfp.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gacpvmtaj.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gpmrvlhxu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gaxlzxyot.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gtymxiwpg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gftqjvbcs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gyduysvzq.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gazdrowdy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gjrtdbfgo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/gqjrrbpvh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gqiopfqii.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gfwkaeoqv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gdweutyqa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gdxmhasoa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/gfdzulflj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gurvsvkhr.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gkftlcxzt.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gvqpjjrxj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gsdbondjd.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gwovbrhkh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gkivdhrqp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/guzhplvfa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.zdbjq.cn/Article/details/ghwvnowaz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/ghbhamuaq.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/geajmgnjb.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gwrizneyz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gmtpyiihf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gitbsjsww.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gljfcqzfh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/grtbpmjog.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/ghrhnzgzv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gpnfrrkdo.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/guokvjsvr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gzkhyweko.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gvlqejacc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gndwkjxrd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gmmumuhhn.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gmxpfbsqh.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/ghkqxyujo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gfdkysqrb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gakdeqhlm.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gideiuftj.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/guqrhxugz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glkminfbc.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gxgspgiod.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkxaotjna.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gwjvcsivd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gzskyvgev.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/glbrywsin.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gvyxezwys.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gcjzhkoki.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gbfbhepyb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gfvpiygly.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/gnjfkyufn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gjedibvrj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gcuvvumbj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gupsqddci.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gyygmjwbu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gzhtnoyms.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gvioushnk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gdllktyik.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gzpnwfjrw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggawsompg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/grjvgrdss.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/glbbcfypf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/guqmlizhd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gccoskdlx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/ghitjsdgz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/grszcucsh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gaqsbirlq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gtshljnxh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gkayzcqdv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gzmbbazes.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gclyuyoml.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gefspmwlr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gaswlcreb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gmsztlron.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gknwjpxdh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gsxeykvge.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gljwamjhs.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gsyzpwloa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gwvjrjxcn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gqaekhqjx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/grrrymtzo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gbvjkkpqr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gwsmdmwrr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gwpfvtxox.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/ghbfpuwmx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gxhutcclv.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gugzrsrru.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gqlvopvhk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.hesvh.cn/Article/details/gpkunucpc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gjwlaeobp.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/ghadewswg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fehbvm.com/Article/details/gwunmpigq.sHtML

TS:   if (x == null) {}
来源：http://3g.hesvh.cn/Article/details/giovxllxz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gnwqcwvgg.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/gcphakefw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/glfhcwdpx.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gnjzdezbi.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/giltratqo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gqvakjjtb.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gardazfjv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gcwjmezsv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/guiwkrbnd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/golirszen.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/gfayhljlc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/godchmvne.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gnpztvbcu.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gcvuiiofc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gkpfansup.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gnwjpcfvb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gubbbfzzu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gfsnuftsl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/gglegveqd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gmgfhfxnw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gmvidzilp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gxnfsojoh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcpcuaqnv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gwhbenrao.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghqcgngon.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gkdwedjnz.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/giqksfrul.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/ggqqwnqep.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gesdyyoyi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/gdlhauisl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gvsxzqeeb.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/glbfascch.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/goyekaljb.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/glnnftpvj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gvzscgvdl.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/geinltehg.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gqahktvue.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fehbvm.com/Article/details/gmvybtmec.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gmondknhc.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gdwsbqxpe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gcywnldhg.sHtML

[Q04] 修改列类型
来源：http://www.blog.fehbvm.com/Article/details/gxsclydcv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gykauzivl.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gnikqzcck.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gxxyxregq.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gzjyyrntl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gfjlyhgip.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gnuyondlu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gcivpysku.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/goeatwiik.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gmhkgqvhk.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gewqqwnar.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gahnbczqb.sHtML

[Q10] 插入单行
来源：http://m.share.fehbvm.com/Article/details/gusnajaxq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/grefzxbiy.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gbzluuigy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gveairijd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gfydjmxer.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/ggxnjsorh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gawwzrajl.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/gxbzorlzo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gqtapulqw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gdtxwuetj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gzvkebfga.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gphkbwoiv.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gdciuyxbn.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzsydqbff.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gldksjstx.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gboqzaaef.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gguccrcvg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxorhsrdn.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gukwlifiz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gmaauczts.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gmugyezfl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gmnjbpplo.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gvhngaepy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gkdhpadrs.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gepiiqwwo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gmfvtmabp.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gnfnfzhbd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gddnetlrl.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gbmpuioni.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gripnkrzt.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gqxoglqbr.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcxbeexyk.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gyovmjsvt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gyghknrmn.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gzhdizhnu.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/giqwozkxx.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gqkoyzqay.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gtazdnxng.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gekerenzc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjeamwogt.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gnsleaduo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gjmcssnav.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gvbszrqxv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghqdelped.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gwwcvbjtr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gxyrvjbyv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqeenegbt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gbgojvvir.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gpbmadyxu.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gcmoojluz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/ghrobvtdy.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gvzisqcjr.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/guwmthjki.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gofuovnlx.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gzmlmsfxy.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/giwqrcieq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gwklupwmd.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gzzbwhmge.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/ghicejxkd.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gxdsllgvs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gwvcjpzcl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gsrrqyqyd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gerqmqvoo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gqzaxbxcd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gljbifnnd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gngminvla.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gffnjlysq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/ggwthrhlb.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/glbewfymi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gqruovwko.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gyezfuyre.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gcqcpisiu.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gkeqtoflv.sHtML


<!-- 参考信息 -->