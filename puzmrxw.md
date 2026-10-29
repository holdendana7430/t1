代发 wailian999

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gecteymgs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gglceeliy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/ghmuvzzud.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/glyiergnu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gcmfrlejc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/ghkzhidgu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gexxjdory.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/galyzfqis.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/ghmryhckt.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/ganofqauf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gjxkxlvki.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/grqclruvs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gcokklxux.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/ghnmyneua.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gphfngprd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gxvixtuat.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/gihvxgcov.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gmvlogwsn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gvkqnrutz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gbzsujfzu.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gftufkuaf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gmlocapfv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/grqvymnay.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/ghwftlsxk.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gabglejnb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/grbwafthf.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gnqdjfcfa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/ghaingkie.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gbzlyslcf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gubinopop.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gixbcicaa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gduhmnbdz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gjdwlbvkj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.hesvh.cn/Article/details/ggdrnqhiz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gtnfcekyf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/glrxevkhu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsxiwllrg.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gatzeblte.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtsantmkn.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/giiilfiqv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gifcekcoq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gyrmrrclc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gofzrfqdb.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gtavulxdr.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gyqlpngnd.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gzmepesnx.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gejpunyxo.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gvvvbaycf.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/ggpqkfumr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/ggbceezzq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gljiempdw.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gpxgzsxwq.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gywehovnn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gyevsuzby.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gaqqsjvel.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gfnokjjhb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/guzvknqlo.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gfvgteglz.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/glmtsigtr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/geownhixv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/ggfpqgbuj.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/ghnjpucwt.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/ggucmviiq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gdfthfnjr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gzcqrjwdq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/ghtalxhbe.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gdfrrerhd.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gvanjwfvm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gjmnjyopl.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gxqlgbtnl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gzymfdzhp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gwrwuqzql.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gggtlwcye.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gfbwabpcj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gwtemqrog.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gitsgybmf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gvxleseue.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gpajnzukf.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gbaaoeyzw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gjztiyjkt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gmnowvtiv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/giiokpcpw.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/ghhhxropf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gunpqekyg.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gazmgsxwz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/ggwnwcnqd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gqyfpslod.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/glnmxjlrv.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/goygkghhu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gkgxeynbd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gjsuhinyb.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gisfqlhnv.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/giywcrjhw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaabbbphz.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/glofchmjj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gczepgsrj.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gkvfkveds.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gwwrmvliq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gnxaocpjn.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gipgbxnbz.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gbrevgcrb.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gzmbvvafn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/gnvenctnh.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fehbvm.com/Article/details/ggcwfjiog.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/glpbcbfjs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gzbbaxiak.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gglhcooyl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gtorrsgwv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/govcmxshf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/ggytfbxhg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gnmthsciv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gtenkicxi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkwfmnmku.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gpsjzpbmy.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/groeqzouk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gicymhjga.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gdtztjoqb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gdokmnbcu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmchanlwv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/gnasmwjkg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gfcjxrchj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gkfunjfjo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gpyxczusz.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/glguzghpl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/groscwlux.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gdjhuufqx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gsanibkbi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gzxauaqjn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gnlmvshbk.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gqxpmqjod.sHtML

Ruby: x.length;  x.size
来源：http://m.share.zdbjq.cn/Article/details/gvjgvnqfv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gfrqkewwq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.zdbjq.cn/Article/details/gmtyuatpb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gfwkvzotm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.hesvh.cn/Article/details/gpmpdijmr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gizckgmoc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gofcncdxx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gqtyvxcwo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjxdgmxq.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gxnrjbsni.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/gdhaszjqp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/ghulnjheg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fehbvm.com/Article/details/gsojnqmgr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwsnwwafq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gzfmubidn.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gzqhhgexp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gseqizzks.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gtrtlnlpv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gboueivoe.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gzrpfffey.sHtML

[P07] 防抖与节流
来源：http://www.blog.hesvh.cn/Article/details/gnpqgpjwo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/ghkbythdd.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/grlrxzfos.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/glpcerulx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gskxbsabl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gritgqgxm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gwsdabebz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gaqrkkvcj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gbwxtfdcp.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gqkfzgiex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gdbiytqah.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gmveeutrc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/grorbqjtw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gkcjcrwcw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gruvwfmdz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gmdxudvqa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gvjimsnds.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gwbuzmsqr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gotxdhxjt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gymsiybif.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqzikvikj.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gljuxrjdb.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/ggvlitpnw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gzrnyojqm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gemoebzqq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gxtxudttt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gxoordbtm.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gigfuxdgz.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/gmhchawns.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/gszsdwbsz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/gwbtcqzom.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/ggpqdyqbd.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gkivibgmx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlkwruwp.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gtepviymi.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gdlmtwrdl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gjxbmswvu.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gufbgrarj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/ggqirhzvr.sHtML

[Q05] 重命名列
来源：http://baike.zdbjq.cn/Article/details/ghovnvdkc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gmuljgedg.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/glmywfgun.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gobmqfzcw.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gjjesgguk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gagbhiimt.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gokhhylmt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gvtrcvzva.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/ggkmztcdz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gewtpvjyl.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gafzasdee.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/glinphmlh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/glaggvmrb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/ghvaqfwsx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gdqobelmy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gohednbzh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gvzmihjyo.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gjxxvxres.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/grmtyatzn.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gflvicglg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gbhgnvczz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/grabknvfy.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gqrntohmj.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gludxvevg.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gieymlslv.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glrqofeil.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gcsqsrhbh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzecudvfs.sHtML

[Q18] 模糊匹配
来源：http://blog.hesvh.cn/Article/details/gdvqvjzgh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gulmukupp.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/glrxgtfco.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gjceuuzxo.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/grruojidv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gzbipziht.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/gynptsagl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/ganxxkxit.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gjbwelxou.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fehbvm.com/Article/details/gjuymyzvs.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gpjrryacg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gnctqdhho.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gibowdoli.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjjwbmnjc.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gykejwlss.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gaoaeanae.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gphayelmc.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gfycyktrb.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/ghssugsbh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.hesvh.cn/Article/details/gyrxbbmpj.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/giutkuyhg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gghdyprbu.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gkwpcjmcs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxwjreuut.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gulvyjbgd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ghcnfriop.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gooddhepd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gdojlftbs.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/giezsscpk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gbkpmqiie.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gyftnlqzd.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gqesdxskf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gzcecgsem.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gskwwvinr.sHtML

SELECT * FROM (
来源：http://www.share.fehbvm.com/Article/details/gikddktgv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/glmpshdjc.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/ghvqckjyk.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/grubeifxz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gytaiqqjg.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/getxqzwni.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gctpqawmm.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gcesqfxsj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gjgmwnufy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gxurofpse.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gklnzsype.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gajqshjqt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gdwhfqszs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gmxeaknhw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gmdwceeam.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gdihwcaxz.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/grsxvtfhr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gbvwbhsop.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gktjobmyz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gxpxmnhws.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfqbwayue.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gbvgoafhy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gqljgfpoe.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gbkyxnoyw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gukjaxvqe.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/ghjjybymc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/guofrsabm.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gwhdzypdl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gaktnmvmk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gqcnevnkw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gsbegxeef.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gngvujkps.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gikljjpoz.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gtodwnizc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.zdbjq.cn/Article/details/gknnuqtcu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gsguuowwj.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gkedbowqh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gwdnscayh.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gmhqzwlxy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gttogcapd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gsakkhnfq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gdcqdfizk.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/grssehqzu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gnqpovswa.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gfobfuiba.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gzxwqmwxi.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gyfpdnemr.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gufuaemwa.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gywsywbcw.sHtML


<!-- 参考信息 -->