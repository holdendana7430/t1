代发 wailian999

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gvbvmcbsg.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gztvkedzi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gwopaeufu.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gwavrmyur.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gvkimkixg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gqzfbtrif.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gfwkygqzo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gibhuezas.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.zdbjq.cn/Article/details/gpetzwdqg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gwmavniky.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/grnmgfgmm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gycyiytqa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.zdbjq.cn/Article/details/gnzvqlyda.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gsjryqjhf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gpkmeroqh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gbktwshmz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gkmbjidih.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gdnyyhjip.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gahewcsua.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/goendribs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gdkrgbuko.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gazukdera.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gvqrhrnyb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gnixphijm.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gffimmfcc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gpmbakenq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gwflundpv.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gwljfzpbh.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gbgccspzj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gjltdulmh.sHtML

C#:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/grfcgqnuc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gmyepqzed.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gyugvltbs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gxtgabxwv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gdhsznema.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gtpzvrcnu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gdgiehcwy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gbtcuifgj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gqlaxenaw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gvguntqtv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbfpubexu.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gdnmdssjk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzmshojqq.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gbpawwydo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/giuiuwjyq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/ggulsetxc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gbpqmlmbc.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gagauaccu.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gugeqlmae.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gaottxoxx.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gwrazymch.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/ggyaosysj.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gwxgypdss.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/glweewasm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gqmdnulaa.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gjhmrbvnd.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gfcysslmn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gcupymhro.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gqfadlniz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/glxeduypv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gpwxaqjtj.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gddiokhfd.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gowwqyitw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gzymngdvf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gtcdntsau.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/grssuivtg.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/ghuczyqve.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gslpkfyjf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gfwzthmtd.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gywrwrnpv.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gehozoske.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gnizryjng.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gsghwrnxf.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggnrfhujz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gnbgbzrys.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gubldpqph.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/ggrofqdiw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/goleeeixv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/grxfsnqsg.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gdyvbkkwj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gjezrnwrb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gbskygqdc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/ggdhfbnsj.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gajfhfggt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gghvswfak.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/ghgtpdkhk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gtwbxpsah.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gxovnilhe.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/ggnnufzkb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gdeqxvyru.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gbjlphavn.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gaijkssdb.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gfuomeotc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gmzqtyqrh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gxvhvcpiv.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/grccdxxcz.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gjjsfccgb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goujelfqf.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/ghjydjzyv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guqypojak.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gfuhhiljg.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gpdrwmhct.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gwwgerfds.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/giqpaefgd.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcrjtwyq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/ghrorzkhu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gkqccjiek.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gtffatnfb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/geaptsqvy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gxuvntktp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/grlrhjwun.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/ganskzlwm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gkawcyuvl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gmjmxuivv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gihlteetn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gvssgaqud.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gieyygfot.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gpckxkfig.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnswwabpu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gwoeeaqpn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gephrscob.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/glpbqckho.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gefwtosnz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gfzetnveo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/grzbrmqlx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gkwejqvyy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fehbvm.com/Article/details/gzmayglgn.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gpduxjhbe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/grxtlvhgy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gvxzmyull.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gdrweavaz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gdvbeujwe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.hesvh.cn/Article/details/gfgxzgwig.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gotdthfyg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/ghwjpurds.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gmjhwfspv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/ggcdkmcjp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gmdpsxhdi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/ghlqduvvf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gqrkzoxmu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gugjjuvxa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gbhhqzvvh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gsakelpne.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gytyegedi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gsoywmcci.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gcmyyaery.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gaqavfjnh.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/ghaxwtajn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gtjivkxdm.sHtML

TS:   if (x == null) {}
来源：http://mobile.hesvh.cn/Article/details/genirfeuv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gunhrixyc.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/godislcdc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gqegfspxq.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gbewtcyhc.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gxfymdhld.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gnldanwfe.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gyqytatre.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gmuggkjht.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gawmpaczb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.zdbjq.cn/Article/details/goiidttqs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gdmknrsil.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/gukzqxgkb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gntiwozth.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gfhwwgpnf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gfnhfnpbs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/grdolnevl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/ghrutzvhz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gfnbmivpu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.hesvh.cn/Article/details/gmhahvpmk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gcoumaret.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gqscxvjay.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gwqjqzirp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpyjfvokp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gpupcdwqy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyohweebw.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gpdglonlm.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gnwmukmjv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gyfrzkspr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gvfcrpmgv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gebfbdkbw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gwgxuyhuk.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/goadptpez.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gxqfrotdv.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gqjslvemi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gpwvpwtpc.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/ggwwqsyvt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/glypzoncp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gvgstngrn.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/glmwjnitk.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gyyvkssrt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gvyotiwyg.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gdvdujwxx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gkxqdiuil.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gbdnpalej.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gogmtzmhk.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/grdavpwpb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gajljgcly.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/ggxxjrmxy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gnpdnlmsa.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gbmzqnszw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gwzjoffnh.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gvrjbqzqa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gcylozvmt.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gxmpzqnqd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gfrtuxexl.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gtdkafwdc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/ghyyxkutt.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gcbgccthg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gpcsnmlty.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.hesvh.cn/Article/details/gnerxgqth.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gypxsrgqp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gtyysoxhy.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gwktcgqom.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/giukufavz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gnqeedgwj.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gqcdqtosi.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gjqhbkowz.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gjvlyqyti.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/getmqgaxu.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gqjsklhxq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gawknhasq.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/guytlymvh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/gxydwdrdi.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/ghraodcan.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkpabbz.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gdtibsvww.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gimxulpuy.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gacfkhmtu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/ghibrvgdt.sHtML

[Q22] 排序
来源：http://read.share.hesvh.cn/Article/details/ghhjopjjn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gwfcgcfuw.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/grxesnftg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/ggefwwtdr.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/ghkdpdjao.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkujcuvsq.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/geokrzwic.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gcdbdnejt.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gtnqmihvm.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfgdqsxtf.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gocnizvrw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guvhmreck.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gbaqjbhcz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gbpjskbjs.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gtdrdblpr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gufkcpvkm.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gbamtbgpb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gvcvkiilq.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gkwrkdqga.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gglcwhhuw.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/guujwhnzj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmfwcwulu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gfdijgmwl.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gkefmaozk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gnicurjhe.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gwlzrsflp.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gjyrihtgk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gelyiblsu.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gbjacyfdb.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gmxnqrdzb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/glysbyywi.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gfddwrgeu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gvqsdwwfz.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gluipydbn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gajaqxasg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gnhmevytp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gdddkcnzi.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gifnwcqvv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/glosoyzvi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gymzfdmsr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gcrdgkubq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gpcvdubch.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gianjygdt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gogvqlnhq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gweskqdfq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gbjnxreup.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvfjyabxd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gxnhaaszo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gdctkthpv.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gxlifappp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gjheldtuc.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gdiztlqni.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gopaosjfu.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gfrzmfihr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/genqnlrir.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gowsunnrq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gycpnzikz.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gypnsdexq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gpuqvcalz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gfmrgeobn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gikmvxtvo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gownpboge.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gjmmhxrhw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gfrwewlhf.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gnyfbazny.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gvmeakbci.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gniatydrs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gyjgxvork.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gcvjbfadf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gsovqnjnn.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gekpqmmnm.sHtML


<!-- 参考信息 -->