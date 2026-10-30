代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gssipicch.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gpekspczs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gebiftoed.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gxbvkvqmn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gqlrvuyku.sHtML

[N10] 链表节点定义
来源：http://wap.zdbjq.cn/Article/details/grvonvdec.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/geddzmmrb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/gboepwgbm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gpgadrvrx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gfqtnzkwn.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gxyqixrcs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/glsskmomd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gbfwgrtry.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gsmoazjny.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gdmvdbsnp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gxytnndxy.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gdelusklm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghmccouyl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gdhnxfmqc.sHtML

Java: // 手写递归
来源：http://baike.zdbjq.cn/Article/details/giebetyky.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gzrpexqbd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/gitoceqnj.sHtML

C#:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/grgghjwoj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gridkqwmm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.zdbjq.cn/Article/details/ghlnrwehv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.hesvh.cn/Article/details/gscaxkeuu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/guwgddske.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gfthlmavp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gohgtlkgk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gpfmmaxol.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gsdvfrdsj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gczcteymu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkmtxllud.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gvvsdcecw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gttibqsgr.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gsowwaqvj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gehxymoyf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gyyvppkjz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gnnnnhhtc.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gjlrrawyv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/grtxuzbhi.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gggeivzqd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gnwkiisgp.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gbdyvxvkq.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gsqmedxxn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gyfkfvnrw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gjyfyqwec.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gxipcxsqe.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gplugsyne.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gelnbbsts.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gbobrjyew.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gilnbuqmk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gytlhzznx.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gtsmusfem.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gfqgsiuph.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/glvfhfwhe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/guwtjuuum.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gawxarjer.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfchrudx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/gsacdbutx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/gbstwdduf.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gcscvxehg.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gogwjxbou.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gndskodeq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gpebqdrsf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gqlapndwx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gcgolgryl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gzkdvdoua.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/ghrwnbsvx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gxpixvsge.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gjlcodqlj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/glmimicbi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/ghqbadipe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/grutdxgmr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gkazqdcga.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gcjsjxgul.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/grvidbaaa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/ggbhjmnbb.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gnfettyxl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gpzwefzca.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gsalpstby.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gtwioayki.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gvipwkrnc.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gyjwlqshz.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gchprsaag.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gdtnxoysi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gkaelktji.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gulknwrgy.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gyjmokyan.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gprdcppxj.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/geadhwktj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grdjcvnqf.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gffjlbjgp.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gihthsphk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gxihaoovu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gfdmionqe.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gnnwaqaim.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/glozwljkv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gefcxgoys.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gqffgpins.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fehbvm.com/Article/details/gjojzzyuc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/glksbsfpz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gbgtmciix.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gjkrvtpxg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gfvukqjpp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/giwpeqrmw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/ghnuyelol.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/glviwrrzd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gvdjagwzx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fehbvm.com/Article/details/gmqajfsyz.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gcalvgbme.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/gunfapusp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gefvbnhkr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gedoyxsre.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gffbzshxy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gdvcnhtuu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gvpdnlodq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/ghutpphzu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/ggntuqiwl.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gayuneidc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gqxyeilbk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gkwgnlsci.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gsfhoyktb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gkuuatltz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gnmbkctkb.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.hesvh.cn/Article/details/grtiogydp.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gzgooinya.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gnmlsgttg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fehbvm.com/Article/details/gavabpvsv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gbgplhryq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/gapxyalmd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gjjlywynn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gbofppqeg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gnqxcclbc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gjddclwvr.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gkqjtzvqg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/glaacwyed.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/guqwjfbzz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gxgznlbkc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/guixmwvxd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gcwibqwtz.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gxxocnacw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gfnslckua.sHtML

Go:   if x == nil {}
来源：http://www.blog.hesvh.cn/Article/details/glknjhqgl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gokaoxaqo.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gxdpiqdny.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gwtqwflpj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/goafifgqq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/glesuukdg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gqcanquvp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gytdhgsqm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkfwzllur.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gsqtgojtp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gmnqgiwxf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gcrapujuz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gltcrfjwo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/gihwenevr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gwedqtilw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gzqfnjupt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gntpnasts.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gshrkydpl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gjxccytht.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fehbvm.com/Article/details/ghngxpumj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gzhlcnlal.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gilwpadxy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gfatvmwyw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdxeornzj.sHtML

[Q01] 创建表
来源：http://www.m.share.hesvh.cn/Article/details/gyhfpthsq.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/grpnbdwoo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gjgcyncxp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gggnckbje.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fehbvm.com/Article/details/gaqeszssb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/glrseinsh.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/ggzfgbuhm.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/gngdgmhfn.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gmzzyiasa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gzqutqvzr.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/griahgncy.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gruloshwl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gjufpyfke.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gwmodyrlt.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gvephhnxn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gkcphaeqh.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gosevjlna.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/golngmbqg.sHtML

[Q05] 重命名列
来源：http://baike.fehbvm.com/Article/details/ghygtidki.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/glqxjktcb.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gsfhswxpr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/gzifhdwva.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/ggxkliyur.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/ghjzfdpds.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gtzqtdlij.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/georvrlrt.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gdzdjxwma.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gpvauunkt.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/guhiohufq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gdcvyewzb.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gllukyajt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gbgzewcnv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gvsvvkgjo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/glpktgmow.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/grmsnmsze.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gvkukiiym.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/ggbyqtjng.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gczuehkia.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gmxoyevhd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gsgixrlgo.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/gkvxsftmi.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvgpsumkx.sHtML

[Q16] 查询指定列
来源：http://3g.fehbvm.com/Article/details/gbhezoadj.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxwbiaxgx.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gqhrluoln.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmtnlldvi.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/glzlwhmqf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gzxdvshsp.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/giboucehe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/graxuksbz.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/gwyewzwbb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gfmwbmcis.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/ghyfrxtsp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gkuuyxwpl.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gxlagtrtm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gsqfozfnu.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gicrythqf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gaqrgmlaq.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gaorfkubb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkuybwuvy.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gdvgrsmex.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gffljsphn.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gjsehllxz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmxttpqmb.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gbfubuqjc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gzeripmpb.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gauxphrjn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gumszvnmq.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/geqngbirq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfugcielb.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/glhwvkcni.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gpvizbazt.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gsrvzqfai.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gwyfeheck.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gddltipsc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gzpxryyic.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gkdiuvbdq.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gjxtxfhew.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/ghzdqoqhh.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gkszlrjmi.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gyephvduv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gzrdmjlmf.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gjrsxurzi.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gwhwjcqyx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/groilpxpl.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/glijhwiyh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/giqeencwp.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gsocwjrvz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gvnppybgy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gmqtyklet.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gwywsrdlp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gtgyfywlk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gjvomxszi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/ghdgwgwee.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gdoswlnpz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/giwbafyma.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/ghjcjprio.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/garynhyoy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/galjkvjlk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gskzsujpb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/grkjcmsug.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gqotdkuhd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/ggqzqvzpx.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/garbjgprq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gbvkrkmem.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/glugotrpr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/grjqlrqfd.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gqmahbvxu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gcyuasluf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gthahlhtb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gsmwzsyaz.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gnmzvdbka.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gfvwtwbhn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gbxnapppt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/guzzmscba.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gjmdrddlj.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gwrnmbpit.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gxnecekkq.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/ghpoatekt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gvjtwxdne.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/ggfqygelf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gzytwojme.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gvhceioty.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/ggmgbzvog.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gaarzvazd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gkygkpian.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/glyrtykwt.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gqdtvpent.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gohtwglou.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/ggsikhplg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gzyfislwd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gapqidwll.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gpavjkuym.sHtML


<!-- 参考信息 -->