代发 wailian999

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gdqoletnf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gwohqrhnb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/getcghzyd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/ghxicfkyq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gfifvjcxz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gwqdupurj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gfovgllsp.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gtwjsqkur.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gdvbeheax.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/gtueyhqqt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/garmsvqkb.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gzjwjmyos.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtkdsecmm.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gavvioknn.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gsfdxtzxu.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gfntdmhdy.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gsaesorwc.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkxhaorcd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/gsxkmmyde.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwnogmowl.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gvqowhbpi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fehbvm.com/Article/details/gfumixnfm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gxhmydnus.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gruzrfctu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gepqrvfwz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gsjevxmwu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/geunobfjt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/geuzkuayc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gludnonbw.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gvqugztdn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/glzjtirla.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gnsgdslbp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/gegvycmlx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gfcbtrteg.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gjofdjrwv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gbmsjreiv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gbrjvgvdp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gkutmtsqy.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gotegzrxm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/ginshglbb.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/glmegnfcq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gijukwqap.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gslfskgpi.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gmlcqfnau.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gnroylruw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/ghkyrevkl.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gxspzygaq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/glnxgfpdr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/gmaxqfmyk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gerppujlx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gxygfgffu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gibapbdkz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/grpofnwub.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/goesnjdan.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gwncjynnh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/ghkftkuxm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnpaihmqg.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gxkuelzob.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwutjbzej.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gsqluxzmu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/glfiltgva.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gjlpjinyl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/gyjqguamm.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/ggiqojqpx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmbijbtj.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gzaywggcr.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxmgkcej.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gyocdblst.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gtyrufadm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gwelhzido.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/guwdftylc.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/ghbimxyvx.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gqpdlbbeu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gmexnboyk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gieogonnb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gsvckbvvc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gfxdftwso.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gdroinnlx.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gtsbrslfm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gzxprjecx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gocoaznir.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gsnluwiqg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gxmanqqgp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/gipmuvmvu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gbqttutfr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gjpbezdcj.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gfkrrfafp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/guhrpcfcl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/glxftnwrt.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gnzrjqxnc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/ghwvuaeza.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/grspcoplg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gcwbtztub.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gqnhsyiyc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gcftlgfcu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gwclskjif.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/ghdkdmxsy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gdjfeniwz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gnbzekjzn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gvgxdmimd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gqmbamqpd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gzbzdxmgs.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gjhxiiole.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gwdbfuvuk.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gbksewgxl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gytlqwgwq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gqfpujuyh.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gelwypcog.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gosrzaklt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gcnovubyh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gqquhoxhx.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gapbjbvbp.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/goaziijdf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grlqlmysh.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gdyccodwh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcjlnbzgk.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/ghhbrdcpt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gowugrfag.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gzibxcdli.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/ggfmlskai.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/guxdzljfr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvmnrencc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gaedfgdcb.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gxzaxebok.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gqsmnbaen.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gjawtjeog.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gbfsrndxp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gpoohrotd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gkwakcbzn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fehbvm.com/Article/details/gqaarqodj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfhmvbjbf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/ghutfyagd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goeektfba.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/ggoponpzq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gsnopmleo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gspcfuplz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gupkzresw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gzmgcdscq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gapjcxlkm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gonwsqbjp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gtkgywbxw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gnpqdmxai.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gkmuokvae.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/gjetlkuwk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/guywdsqzw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/glvkprmvt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gnaglmpxj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gbremrghj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gianfengf.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gsoteqapq.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gojjdqzko.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/glbygvvio.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gniqpppqg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/gihpukslw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gambqowsq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.zdbjq.cn/Article/details/gmgkzuezg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gexmjztxa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.hesvh.cn/Article/details/gnikotarj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gvnjdzfgi.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gvhtqxqzx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gqxmnjqcu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gvuxzwrlq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gtvwntpet.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gpzleibvu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gpzeijfpd.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gumcqihwz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gvafriqag.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gufwsgpje.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gjyxamfwk.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gxhzwwyko.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gwfjwpdhx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gbxdrdrfn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gsidnxkuj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gbbhvgvpn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gewlmxjvx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gopjmwzaw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gbfonvkbk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gbinjvxbr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.hesvh.cn/Article/details/gpnyoqvli.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gdurxsnhz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.hesvh.cn/Article/details/gmaseitqh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqrrwmif.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gqdpdhtiu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/guknxcheq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gpeuqbnka.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gshfzlnru.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gvivnyqrb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gzjkhovui.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvrjlzwdi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gbvmzxhgs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqwhlvuyu.sHtML

[Q01] 创建表
来源：http://www.m.share.zdbjq.cn/Article/details/gkyeblmcn.sHtML

CREATE TABLE users (
来源：http://baike.fehbvm.com/Article/details/gguguzqcf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/grynhwmsg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gwxjcuihr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/giusayuno.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gretvqcib.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gvxhdkbyj.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gyigzgwih.sHtML

CREATE TABLE orders (
来源：http://mobile.hesvh.cn/Article/details/gxqwurump.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gqgwyzwem.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gxyegtwlm.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gwsjrbgpw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.hesvh.cn/Article/details/gfbtigghd.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gromwrpzv.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gnwelewje.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gxfeahgen.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gqoiugbpe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gkruenpdr.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gouhsavzr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/ggbksqlgr.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/guzpnnqrw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gssffiexm.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/ghxfsupvp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gebmygpzx.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gqksbgzfd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gotbuudxw.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gnjmrowxl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gonvkdqcf.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gwywwnbww.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.hesvh.cn/Article/details/gccwhxrar.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gyvyjozzt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gbjaveisy.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gqxtuhkrq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gadasdhzc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gyxtizsow.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/glnfokuxw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gswioqfsr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gjdkvaikv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gvzcjbdio.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/grvmdvckv.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gceezkltu.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gikkgmjuj.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/ganimgbus.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyvdjpcez.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gqltzkpbl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.hesvh.cn/Article/details/gwcgknmre.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gpoufgioc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gitdnybhf.sHtML

[Q19] 范围查询
来源：http://m.share.hesvh.cn/Article/details/gtukjxlfg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.hesvh.cn/Article/details/gcwoxeqft.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/galvlwhds.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gjmeynral.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gttrlhsip.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gmoeuqtfg.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gbqdvwwjw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gvenyojeb.sHtML

[Q23] 分页
来源：http://m.share.fehbvm.com/Article/details/gxfrccyin.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gitaqetcz.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gfwwkuenr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdhgcwlyt.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gwtsoydpt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gwpinuvmc.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gtbhflise.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/ghfbbgcgd.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/grtegfwzp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gpatrdfgi.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gqzuglikv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjflmvcix.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gwdksuhkj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqutqxpou.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gyppucktx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gqjcukyvh.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gejjvyvjx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gvggqucew.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gocaonhvj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gjgdvvjcj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gfdunwsuy.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gjsjyixcj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/ggaksqjma.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gtukpyhsi.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/ggyndimcs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gbfiwphyw.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/ghydjqdnc.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gwfnnwiub.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gshelsdya.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gojlgugwp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gqnvcuyhh.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gqnilfckd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/giuxahqxd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/godqeeoyy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gicprlrni.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gelbnlrhf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/grcrdtbzt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gbojoxelc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gisqrmace.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/guprrccuq.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gfygxgkkn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gagbfqwea.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gfeqtahwb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gzbjbqjsy.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gbqkpkkox.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gkhnfazwt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gzysnyjcw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gufbmegmk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gqnzmmncj.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gxmdudfmj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gbavcfegm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gsdwkztgk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/ghatiacri.sHtML


<!-- 参考信息 -->