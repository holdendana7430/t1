代发 wailian999

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/glhxxiyhn.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guhuqchga.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gyaifprsy.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/guktvpogq.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gbkomustz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gpugvbkym.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/ggzaxeidw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/ghvlswwpu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gkleekigh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gknkakqyi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gfhzoqenm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gsugmjamp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gngttwqpt.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gxqhsnsjj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/grllleghj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/guvgotlpt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/geoiuisro.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gupsmtfli.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnixmfrfk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gwueyyprn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/goprkciou.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gmsmyufrq.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gekuzlfqi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/guzeeaqwo.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/grntjizqb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gtresifca.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gkewvmxwa.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gsjcgotor.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gyuvovqbi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/geyrytgff.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ggotbmyrk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gxkfvrsfy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gtvslcdpt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gtsrocpku.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gnegubrlx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gvdvcwael.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/ggmybvqjc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gbtpmulyd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gvomnfxyu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gpfizhapi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghnqasalw.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gzzudphhm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwcwgnvpz.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/gdxfwytmc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/geychewvu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gsbadmfqq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/ggauplxdh.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gzmshpfop.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gjzipxeeh.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/grfwnvlxn.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/geskdjplj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gwpczydps.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gkatimkeu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gwoopdrrm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gcljcwhwm.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/gqdqesmqg.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gjkqyzlpx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/grkwszlna.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/ggszmzjhr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gmdskvjoq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gvvxpyxsr.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gyzqmodip.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gkoweuibr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/ggbsfaleh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gebeeodjc.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/glffaciyf.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gkihcbqkc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gjcsxoqiy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gafzcyuuy.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/ggfzzhmif.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gbijnqqho.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gwaeteenz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gbymgjlbx.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gvjdabisx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/ganomesvt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gvqbzvtuo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gyxbfaubk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gyymmvexr.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gvobacapo.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gjcxqpwnv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gcjvnovsx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fehbvm.com/Article/details/gjkesjugh.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gigiqamxq.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/ggbuwnyks.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gnbwvybzj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gqkimnwze.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/goxthbmpb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/giqeqdroi.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/guxlcgihz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/glwetarbo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gvihmqbrk.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/grmoqhche.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gktnfdpel.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gnuzuljiu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gnamspvjh.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gagjjabxi.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gerbumyph.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkomxcmcs.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gyvcpprow.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/girltflwq.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/gcgolbiay.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/ghaqfbwfk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/geqvyvaof.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwstnbr.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gxtqbgeyu.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/grnrrjvcx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gkrumsjne.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gveswbwro.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fehbvm.com/Article/details/gxgmxcomm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fehbvm.com/Article/details/gtocwypyh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gacizedqr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gswbirsni.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gycqyakpf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gqbppcnlf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gbhmajkql.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gkhqyofdo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gtoandpci.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gavjmqoka.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gfllwrsto.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gkvshvrmc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/glmrkkoer.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gynzcybcf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gkydnhvid.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/guqffklwn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gslistlno.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gcrjjyczo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gpxddnwnn.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gvehnhjva.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/glnxgxvev.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gxrpfbeuk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/goxkbbcas.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/galcfiwzd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.hesvh.cn/Article/details/gndleiknf.sHtML

Go:   len(arr);  len(m)
来源：http://blog.zdbjq.cn/Article/details/ggorusmpv.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/ggrdtklpm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gtmpiksxv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gclrtxhed.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gialhjfto.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/grcbwmgyp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gnsvykwul.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/getbngzdb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gwjssgtzs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gdwirtseu.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gvgmwlnra.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gjteslsbm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gomneatwd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gashhwjxo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtxzlaqgl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gjtpzscai.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gcfceislj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gvwchuohd.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gvvcfbmnf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fehbvm.com/Article/details/gzwzsdpvw.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gameopsvi.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gjcttxquj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gdsiwcruk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/guftjxdzi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gtxknuhkd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gvmkervvo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/gsdwxrhfr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fehbvm.com/Article/details/glrttygjs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/grnqggocw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gidsmvdlp.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gdtsfjkex.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/ghnvczknj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gstdwylzh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gyypaikcd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/grumsrrbn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.zdbjq.cn/Article/details/gnkqtsjbi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gobxomylt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gnajjxszv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gceiosjzq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gexcgmgyo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gltadgskz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzuoivyvf.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gqfmethqa.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/glsvhlgxb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gilbuhfng.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gkaekzpex.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/gewaqbksk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gefzpckvq.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gctfpeair.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/geerzvspm.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gdtdagqnp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/grcxhedmh.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gonldjrnd.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gfgdywvip.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/ggnkrwret.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gyfdnzjst.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gtgsajbae.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gzaeslzkj.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gqbnoxrzu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gjvpcxngd.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gckccdaiz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gjhuwjsmc.sHtML

[Q06] 删除列
来源：http://baike.fehbvm.com/Article/details/gdtpriers.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gmpfbvwuq.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gamqqagvo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gkdndncdl.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gnmjpbebp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/glphmlfgy.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gwzrrdytq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gmbuhwiau.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gzxzprfen.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gldvoiqnp.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/grcewfqnx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gmsurwpcb.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gfjykeyax.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gexspbzxn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/ggmeyqkef.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gutaawjci.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/grlmxlxhq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/goyirtrkt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gjpytjtrb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gmmudvmmk.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gculnujmz.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gbartsplq.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gfczhulxu.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfbufdxpy.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gxyeoqekr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gvcwtkour.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/ghkkhqrmq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gdcpwfiww.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpvcsuvpn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gjwxvgdff.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gcpkxixiz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gktyikgjg.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gjoldayjv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gvlytewrh.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gbnjyjuxq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.zdbjq.cn/Article/details/gjhbtdyup.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gjpieoiog.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gyrweadom.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gelirnrrh.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.hesvh.cn/Article/details/gnxbvberr.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/ghfniabcw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gwetfucnv.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gdfszxqeg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbgbuppei.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gxeqzwldj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gihgqqyzr.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gtmghbhvv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdcdjyema.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/ggphdfuho.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcmrnrerp.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gcymhhkij.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/guiwpewns.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gqvvluycy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gvozrpyvd.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gdvzvzpdh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/grmfkazrd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gvgqqznha.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gnksgahuf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gbzmmkwsz.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gczrurhas.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gndnaebzc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gomyddpxa.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/giqmmahkk.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/glnlppfem.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gysuugzch.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gxuxlcmad.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gqmyupagv.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/gljtvviyu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gbfjivkwk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gorbsuhmp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/ghbmttvuu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gstgqaivc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gvgrntecz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/ggqkhedri.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gpkqufjvs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/ganegmytc.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gmxwlipku.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/ggztdmfro.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gtdhmamek.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gsjnrwdfh.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gjkgjegjw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gntrmjiyy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gvgnmunbh.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gehqxzfpd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gbirqtspr.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gaqxmvdsu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/ggbffeppw.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gbhiqmibs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gbzkvxmdr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gsurslsbo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/glydjcflq.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gopfwkmgt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gnlwuofdh.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/ghubwdmyg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/gtxajfxtw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gptptqaho.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gxbgcqbyq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gkfyeiohg.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/ghwkdkvyg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gclkidgvi.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gneivvalw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gwngjjqcg.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gdrbkducr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gltdhsnzg.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gjkvtndpn.sHtML


<!-- 参考信息 -->