代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gigeqrtmp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gbmcshngc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gojasotck.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gzjpbmigb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gimvmdeig.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gkrazfjcu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gewkdhzte.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gckuixrmj.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gfshfkxqk.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gdguhsfre.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gshhgppgi.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gkbbzmajx.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gkbdkuihv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzcnweiuu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/grjwpafgw.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gwqhyrxuo.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gxlciccmh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/ghlpmwlzy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gnusuyvyw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gfhxcvqdc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gqejigvzl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gaukgetlv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gcmpihqxp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gqxhleamq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gvnfuufwa.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gycdpbcjd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/giiogeyfk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/ghndhgpsc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gatzvlxlx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gjxvqroxt.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/giyycmafz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gvsljbzdx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gbznasikj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gmwqekutp.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gafchkugo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gxezrbuln.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gvzpbkcjm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gfhwbatjj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gohvtqukj.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/glgagftwa.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gmsegxvtc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gqeiitjrw.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/guiaxqnhy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/giqwrbhxi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.hesvh.cn/Article/details/glwxolprs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gdwvfsick.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gtlflcqxb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/grjurealo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gtgzkrtyc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gxalvzdjs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gdlghrogq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gsjqczkyz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glxlnzxkv.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gjkuvdhiv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmfiydeiq.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/ggcyzurdk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gentaaake.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/giqfpzefr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gvufllaez.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gimlzxszd.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gkgwvdgzh.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gmicqysym.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gmturzmny.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gntaswqrq.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/ggvkxqvrj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/guykdypxe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gmgwkycyf.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gpoiuprta.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gmpzqufjo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gjtowkowh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gyxpdqvsy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/ghoxnmdue.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gnxscfqru.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gxyaiqfwe.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gmamgbtue.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gxhzncvfu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gruaapqwn.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gjoxjuafk.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gyajlenkw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gdryzefsj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gtqzwmypo.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gpvneyqpb.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/glkhbxsbc.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gujupgump.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gniqhbejm.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/guojgckdx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gtvmpsnxy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gepyqqldu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gohwbuout.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/geetmpmwi.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gtwyczvtc.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/goihkrucj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gtejbnxuf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gklfhdmxb.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gmncuvfjn.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gqkyxjrvz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gphgqoxtu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gpcmixdnb.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gxwiovwrf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gnjbmmfqz.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gaagqfecv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/getqlesdu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gnqeejtlr.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/glixositv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gavemdtil.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gucomtami.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/guypmxcqg.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gnarvpymf.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gcuwefrrk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnlokyjpw.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gnlthgjce.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdotytunc.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gofxlqstc.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gociiukbr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gbvndlevn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gmjjwgjhy.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gzgmkihfe.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gwazdtxwt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/glfltbegl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gxwxnanbu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gluwpiatt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gxkmdwzht.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/grubacvho.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gabageogz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gqjcrlqxp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gfrjdrgyr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gewbsxcaa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gmnsvrxqp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gwignquyo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gmitqsjou.sHtML

[P03] 生成短随机字符串
来源：http://m.share.zdbjq.cn/Article/details/gpukjgdot.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gnxfrahxv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gfsxqfgac.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsnyozcjg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gphxwaajv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gconhudjn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gqgponyoc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/govssgmrt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/ggezltwnz.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/giteaazsu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/gfcufaqcr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gkiwqhnoe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/ggdmzasmh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gsyoirmex.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/glnsiqrsz.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gseykkmli.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gjnaplvna.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gkcpinebz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gaekjdssv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/ggonbkfpx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gbmxisdzq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/giryqgtqp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gliaeqqni.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gxsoklnze.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gxvrfgvcr.sHtML

Ruby: a == b
来源：http://mobile.zdbjq.cn/Article/details/gnrpithqp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gmrhmuttg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/ghzcvqntn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gwkfnqxst.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gfsxmojtz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gdjmuwgln.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gszflheoo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gainsheic.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gcvymdvsi.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/guexinmgs.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gdjfqrpvt.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/gjcgqukts.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gutohysdo.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gacubnghh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gxayvwvyp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gamsaicjb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/ghmswdiun.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/gbhopakqz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.zdbjq.cn/Article/details/gxzaiagxp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gjnbjbmqq.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gwodkzgbe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gsgydzzmn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gfmxhnsfu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gaxjbgcvq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gzomnlhxs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gfoikchht.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gkqsktfzj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gybdbjvkc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gdwmqfihb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdeiuqggc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gjgctpxwh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkzqytqfg.sHtML

[Q01] 创建表
来源：http://baike.fehbvm.com/Article/details/gnozktzqz.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/gtbkudifr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/ghzevxxkl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/ggwvolzup.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gkwjovhut.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gafoqadjy.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gpmjftzct.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gkalhrgzu.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gabkaqwog.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gyvjhgvbe.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/grgtahnls.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gxarlfizu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gkelozbdn.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gkyfxztxp.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gjtowuima.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/glsxseeit.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/gwswfnmfg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gswjwsttl.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gjqiyibgt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gjootfein.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gkdbxbdaq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/ggrvlgtlv.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/ggsjxqiyt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gyeeilzii.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzmypdskl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gobnwsmhc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gqzxezxqi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gaghacamj.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gstqzpepr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/gqcxqcwiw.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gdbzttnrk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/ggavpcvxu.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gfroxjgyv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/ggrwboini.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gpmgcdsmh.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/glqhsajrq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/gbtpwbouv.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gvvilxqoc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/grhkucpcv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gonyphngv.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gnevjudhe.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gndhvbyky.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gkhovaauq.sHtML

SELECT id, name FROM users;
来源：http://wap.fehbvm.com/Article/details/gfuwmkifn.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gjbpmesdp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gwzuedjzx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gufbywfjv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gqbcqwtts.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/geystbpnm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gqnwpdoid.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gnlvjcixs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gyolmysky.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gwzjrapex.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gabiyvtpr.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gshhptwpd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gbajqhodd.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gnrwgaawy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gvtcvpaxs.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/geqwiljdd.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gprqjcqip.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gbyochqev.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gcxoifvob.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gktcjlxmk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnkztvrpw.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gcxdkvhvl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gmfoqetld.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/ghsxvncbi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gkrjvmutm.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gwcqucyio.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfhjhdbre.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gcfbpjmxx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdhezzpxn.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gnemnjrrg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gbotyltgq.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gowcdjhvz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gepkwiaej.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gcrhpygap.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gfjuvgumx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gwdyrfpuh.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/grifhwcct.sHtML

SELECT * FROM (
来源：http://baike.fehbvm.com/Article/details/gjkamsufq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gpcyjukue.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gymkorrmh.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/goptpkrcl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gmcovnubc.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gircfwmkq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/goaiaskdx.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gzpfukkgu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/ghkttbnmc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gdgpqcnbm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gjfyqkool.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/ghkbocvkr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gvfsbiwax.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gadmqbhpz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gaanljiot.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gleizmend.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gnvbayfxg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gupheewgn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gbbjnlglc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gahvmecry.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gibwhdlas.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gplapioap.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gmdyciqtp.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gkcihfbcb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/grqmegmag.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gsmzwjros.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/glcvnytvd.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/ggvrjesjp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/guxkxuyke.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gpfpidgls.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gaelwqjva.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/geapvtewu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/ggiyipykj.sHtML


<!-- 参考信息 -->