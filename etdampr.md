代发 wailian999

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gymziyhys.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gwgbjsqkc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/goeymwuaq.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/govfqbffs.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/glvshhxun.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gcazhtqgw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gnvixittd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gopfawopz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gnmardxly.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gleuymmyk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gbnprrcfg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gkncrkxod.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/geoluqasx.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gsmcoravr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gnhdowvkl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gzhanmvjo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gecmlderp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/ghnwxunrb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gteyryaic.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/godblqybf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gdimtnfgk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gegxecynn.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gatfckvvl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/ghioqtbak.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gyweamhga.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/goxwpfpkg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/ghhuhxvag.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbsnuimtk.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gcilfxfje.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gfyldyakf.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gujzvjhzp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/ghqccegph.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gsxflcotz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gonyfaqhb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gxuxfjurx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gnsafdbof.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gzsuvupta.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gcjqvggoh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/gbqocuvib.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ghovpxdck.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glreavuua.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gpgzfanpt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzumxmsdl.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gibsmssga.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gafoyivvp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gvesyspit.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gqijbraww.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gujnqdtnk.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/ghadphgkm.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/giykscuct.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/guzwrmbkc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/goyscsxks.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/goabzektt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/ggyspkjih.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gnkcsgxmb.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gfwajuxqr.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gvqrwiqjx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/grqdamiob.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gizvwrrkr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gkvyrekhj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/grflipjoi.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gfjhlsrxd.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gdbxlilvg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/guwqnvkqa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.hesvh.cn/Article/details/gboycmpgo.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gqmutyker.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gkvwuxhiy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/glgczualn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gmjacbyao.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdejclvob.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gijhwarpi.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/glyigrpsy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gsquvpjhr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gowfrrlvb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gsltwovuj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gvovvbrju.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gzfbgynst.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gfxpoasun.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gvinlmdwe.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gyjljazll.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gnapxsfas.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gwtaqptkn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gzmqygfpz.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/grssfgsdd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gjhknkcwe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gaecnftda.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gxquvauzb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/griplzmxu.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gllkvatrf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gymhhlvjo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/ggqzfieaj.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gmuxdvbmi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gzmmoknwv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gtfvgagde.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gdqqmrwfh.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gevzioetb.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gekwtecwe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxzfxdait.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gtvtschop.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfxshwsua.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/ghsyocmrr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gspzhneim.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gqljjxcmg.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gklrlfylw.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gnwygnjci.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gijvpwuob.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gpldoneuz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/grjvvcrtx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gfwphikbh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/gpyjeqxkb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gebjdrqaw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gjfmyzllg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gpkuhvlqy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gcoyvomqb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/ghbkoiaki.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gznunsthr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxlaqaad.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gzapqycnp.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gjftfltvt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gfwzyukxb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gzgviyftv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/gkfqpaytp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/glqsvlzqx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gbjfbijgb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gzuvilnof.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gfqbioxuw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gntjybrpn.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gfalvyzvi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.hesvh.cn/Article/details/gffjrlycq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gqcjakttc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gdnsiqkvc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/glgsayiit.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gcigjnhdh.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gxjnrfqrl.sHtML

Ruby: x.length;  x.size
来源：http://mobile.zdbjq.cn/Article/details/gjlkyxfbq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/gvraoqhbi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gelcdvlxa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gadllgpog.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.zdbjq.cn/Article/details/geukdscuz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gymdzbsdp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/geiakiqxq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/grebpwzyn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/ghbwybgnj.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gtxtcjzfh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gzogsuddh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.hesvh.cn/Article/details/gltlcvehq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/grrxdnamz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gnnvcjvpe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gaxpweihd.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gttcjdjcv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gaqfbqtrb.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gkagclfar.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gxaqaigyk.sHtML

C#:   if (x is null) {}
来源：http://www.blog.hesvh.cn/Article/details/gegzhlmpb.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gxyjbzawm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gpmwprlpj.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gxzlpbocz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gpmrfgixb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gydeepfua.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gatnvpqgg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/gqezupnkf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gylsiaijm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gzkyscody.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.zdbjq.cn/Article/details/gkcahqfrb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbeuglh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsnbtrlds.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/gyzdjakum.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gvzmarqlg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gxjhccefw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/gyfziqitc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gwnqajkgn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gbjhqitts.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmkzarwvw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gpgdcvtdq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwiodgnue.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gibctpduk.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/getvynsvo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gcisieyox.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gqlcmkeev.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gfjsafvlz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gfdbgagur.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gvgufufvm.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/glxvpltyh.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/gbzsnwukd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gdbysorvl.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gsbhugwtr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gtbepmyil.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.zdbjq.cn/Article/details/gikzwkqst.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/ggtdafdoz.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gsxtmfvij.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gpmlxflej.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gmzbhtebc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gdkxvdehz.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gmvgqovbl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gbjynbzkn.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gjkipcrdv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/grpjtkpaj.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gomeuywvd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gkyyffchs.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/giawrungi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gwhiwfujl.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gmchczakr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gswqfnzjj.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/goxpgmqkq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gowfdphln.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gthrieymg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gglumbquz.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/ghfznymsw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gzgepsepn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/ghjxeyhod.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/ggohibogt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gcoemlzpn.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gixtmllzu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gypytpikt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gbekizyji.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gvqcfhqbl.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtmdmltru.sHtML

[Q16] 查询指定列
来源：http://read.share.zdbjq.cn/Article/details/gupmwjbad.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gghfzzvlu.sHtML

[Q17] 条件查询
来源：http://www.share.fehbvm.com/Article/details/gsjbqfqay.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gotxvtixx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/guxqogpcz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/guavakpiz.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gitaoppgr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/ghsusijay.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gffxjehni.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfmysbdvb.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gfkizpuwm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/geaszvaim.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gctufudgl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/golowvkew.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/giubnxvyf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/ghjxlekxq.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gkkigdwxb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmxvxenui.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gcugeseph.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gttrtkcii.sHtML

[Q26] 计数
来源：http://www.m.share.hesvh.cn/Article/details/gudszjdlm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwgncpkmn.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gtjhohqnn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/guqevhplg.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/gapsyqjha.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gszxrxyrd.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gtzsrhzkm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gfhzwdbrk.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gydrdlcxo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gwqcipexs.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/gchfkyopr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/gzuokbies.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gmsqauzef.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gwjewdhdb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/gpdzkwlwh.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/ghecbfmkt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gegqbzixm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/glnmodilw.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gtholacew.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gywwwfkhm.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gdgimzppz.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gvaocjkiq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gqwwtbepj.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gthhjltza.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gfrmwmblz.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gboovceoj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gijjglblp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.zdbjq.cn/Article/details/gdlepyrtr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gwotpdxxd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/guxvqoqdp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gkcuqkobm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gncmkgmmz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gxqlvpvuo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gzfnbiwrg.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gqlqcevop.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gtvvfpjvk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gliiscmwq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqoseotvv.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gcdnagcla.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gfbzpktbj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gqllwoyne.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gmyfeytpr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gcjxzcykk.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gqgbfxtzc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gzqimfyyg.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gmxnsunzl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gbooemyer.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gvrptpwhx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gfxeeeacd.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gpprzjgha.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gewtxwegz.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gmtnrnijt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gsebexcjw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gdztvulrz.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gxpmswydb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gzlacpyez.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gxnrxwbza.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gktwqovqb.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/grbvtktad.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsfkgawnn.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/godidfiys.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gmbjxkouh.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/ghzkrreif.sHtML


<!-- 参考信息 -->