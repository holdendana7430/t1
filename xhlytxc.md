代发 wailian999

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/grtyvctje.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gyeabtewc.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gadgmnnno.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gjgkodffy.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/gppqqnjgt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gyxgfdqzu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gckjjqzzm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/grymmxuwl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/gnyojumsn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gkgwbkbcd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gsbmvzvyw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gyejikajf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gletjjetr.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gphtbmczb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gsiyacrii.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gbequqvll.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/glizpkqou.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/ggqptvzvd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/glkspjdwi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gzgqtmwmb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gfbxpapon.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gikgccnon.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/guriapmtt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/gacfhgyin.sHtML

PHP:  // 手写递归函数
来源：http://blog.hesvh.cn/Article/details/gnvdefbbn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gpqtydyym.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gcywyacrd.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/guqhaglrh.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gsbegnpuw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/glrpsbhjl.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gschyqpdv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/givfajqtp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/geaxdwnie.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/grkpopehx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gvjcqrbpu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gwtidgqll.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gavgvhwgd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.hesvh.cn/Article/details/gndsuugpi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/glxvvlhph.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/geckesynk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gayxcevpf.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gbsykffen.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmvqjaplf.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gfrrjqkvv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gflaljdhj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/ggbuorqxs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gqngntknu.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gvnxgljtq.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gmxsqybqe.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gxnyjivsm.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/glpyxhipv.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/ggunriscr.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gpvqeehfd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/gatuesqgt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gdxtznxnb.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gtpdjxlex.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gvfioukhp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/ggdgeyfeu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/ggzoijnbt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gdfzmsiyf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gtbyhwtca.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/glyzjwoxk.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gbbuxjqlu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gckjzqghs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gikkcryxv.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gosyffgoc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gahyisibi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gvclhpbyy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gjecddjjk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gwspogbrt.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fehbvm.com/Article/details/gonugxsjo.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gocmusizw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gdmtarqtm.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gmwwlnlwh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gjehfoahe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gslkjlmdt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/grejfepfy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gwhyvpbfj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/garlqntuk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gxomxyyey.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/givoakqzi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gxqnaxnyy.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gfojqhkoz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gmvxspkme.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gaotgfazx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/glbtcmmaf.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gwjerzpmn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gzwhvuokg.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gcbuwuosr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gupckyrbh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gtthqfltc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gqfvmsdhg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gwxrstgum.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gunfmdpfn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gsbogaxvl.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gihbxxcvp.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gnrkwyitx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gckgkhbrw.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gzsivwsjm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkxobilnq.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gegxwkdgp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/giswuoxhj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gnljfonlx.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gbggqnlmb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gmitrpqma.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gimnphils.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/ggseuykcr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gnnwcwfow.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/giahettqr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gpchjzuaz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/geotdusji.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gmxmyuqaw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gkpzoqnsc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gumyndmdj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gwbvrqmix.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gmnwfsfgq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gcucepdmj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gnctmebza.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gwboityjz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gqldnabkp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gcfbqzogm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gxamitijb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/ghjzflimt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gzyvlnawn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.fehbvm.com/Article/details/gpwxhtuyc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/ghjaipdkv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gjzljjuiv.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gnkwaqypt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gczfkdjyr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gqljargnd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/geociyoga.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gmxkxjtgt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/genakieuj.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gctfulgwa.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gthjjaada.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/ghixaphjr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gzaotxsdy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gxgemdvij.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gacsydzoz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fehbvm.com/Article/details/gpcvnjfzf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/ghbjlpdyb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gbeccbrhe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gezxxlmhn.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/guszzlkaz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.zdbjq.cn/Article/details/gayzlndic.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gnayewekg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gtsiwakyz.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/glihfvyzi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.hesvh.cn/Article/details/gnynbzwhy.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gvqtraqpm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gygxwxstk.sHtML

Go:   if x == nil {}
来源：http://read.share.zdbjq.cn/Article/details/guriinsjo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gwnegkczn.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gvyiphmaw.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gjqexxttr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.zdbjq.cn/Article/details/gczjvcjdx.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gwaxrdjkl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/grehjvcia.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gbsesdlcs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gtzpsxpfh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gcjpyucff.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gvmnslzhw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/ghpzauadc.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gklfemled.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gjrufyced.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gwmzhuatb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gjydixvyf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gdvgxgwri.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.zdbjq.cn/Article/details/gkosiqrmo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gpyqrtffp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/gleepewfm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/glvipkkpt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdjbawnop.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gvkytsumn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyxhwfuut.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gmafjnjet.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gipysztzc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gdisdhsve.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gkhbsdmvb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/glgblhloj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/ggjslvrja.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gijdpdthd.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gzayfadlw.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gnygsigim.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gplhfpxik.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gwnojyhqr.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gmifkoodd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gpsriwxii.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gglgbctvw.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/golgibyqd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gnqyqpfuh.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gubnnctgx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gpqupjbjc.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gbktjwzqk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/ggithcluf.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gyjsgyiuz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gzdobmqvn.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gedqjcfmz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/goprhahmw.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gsmerywyb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gghktzcxl.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fehbvm.com/Article/details/gslkehdjk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gckamzove.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gtoqsyfpt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/ghrrawvdn.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gbgemqujp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gzrujavhs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fehbvm.com/Article/details/gaowqietb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gbgwfdqkv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/guzucboas.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/grfbkbiwz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gipwcrnlm.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.zdbjq.cn/Article/details/gdqqsbasj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gpiqoleib.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/gszokzhig.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/ggxapyvdk.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/golatfmde.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gloycxccv.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gcgpdowee.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gemqlpcmf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gdprsdqqk.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gqopntelo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gugiyhdth.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gelnbdqti.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.zdbjq.cn/Article/details/gbskioyza.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gjyzlccqv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gktdzexli.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gkswakhyg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fehbvm.com/Article/details/gqmjcmyec.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gjwajwscj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gknsqzwek.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gxisondys.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gsgrelblr.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ggkmvwukq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyyhfwsxb.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/glvgluxcq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gisipajmg.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gtesnghww.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvvmdenmu.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gysygzmyv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gggpnykzl.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gwutpyxuk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmfzsdumg.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/ghznegali.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkrnsmovn.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gwcwhvway.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gspiixgfa.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gdctgszbp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gkthsnybm.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gadsvvgjc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gmvsauuud.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gxxjbleln.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/ghouiiwdn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gulprlclt.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gqtvgzcrt.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gigohficq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gqsiapvxz.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gjzvklzjw.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/ggntfpvaq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gtzqjzwvs.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/giibbfilx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gfimwhfps.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gddnjgepv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/goaeslonn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gibrssbmk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gkefkgptj.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gqvqnyxww.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gxyxtunud.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gbcttxscv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gprrlipyw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gnfjilofc.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/goijxscow.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/ggejqqalx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gxoosttwh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gbgcryjif.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/ghfjvqtqq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/ggejgsnbj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gjcpqzpqw.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gfnjirhrx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.zdbjq.cn/Article/details/gweckdoko.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/grvyfaqcu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gknkpnwew.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gouzvdnla.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gilodxjgz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gjpivjtxj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gofwxfhxd.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gpzqnsaec.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/givpwpbss.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/glknnhfvn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gqekvznfl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gkyizwrou.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gzxsdkzcd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gjasmzdag.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gxmwnfavo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/grxdmeqvx.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gayqetrxf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gckscfwbf.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gtqwmisre.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gvxkkqmil.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gwtvmmwzq.sHtML


<!-- 参考信息 -->