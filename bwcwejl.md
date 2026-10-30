代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gvvttocwh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gxpydcrnw.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gibzicfvj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gqvjivcyn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gwtxklkdr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/guonurcuv.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gvagtoxlo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.hesvh.cn/Article/details/gdiyvqwut.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gwmxwlano.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gdsgfgbjs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghmighauk.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gtrmjxocy.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gvebnoyuq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gzlhwvutu.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gjpklulia.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gqvmmgzzd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gvzcmzhma.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/gwzrrcvqb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gneilazng.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gfjhivuyh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gmxasjugo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gzcpnvwzt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/ggowpmqad.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gsmlrrixi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsiboomyp.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gxyltntmm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsgvhqbuh.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gglmbuhfz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gfevlceus.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gwubeqlar.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/goadlgowy.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gczatpgac.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fehbvm.com/Article/details/gjymwyszk.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gnigunkzl.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/goazcrjxk.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/glfuozbkc.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gxcdkmxis.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gawtfffgv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gxfocdfns.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gkoyexpvz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ghraimyin.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxhxjfwb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gahxlvvgu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.zdbjq.cn/Article/details/gognydhve.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.zdbjq.cn/Article/details/gcbyzqoaz.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/gteitzhhi.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gcubcrowz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gcoqrwkfd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/ggwwbnqrg.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gqqkebizs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gpqrjzljl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gsnqlzlwh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gifmqwnvk.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gioiunghb.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gsnmxjzgb.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/ggrypqjdd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gekkmhjmj.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gcoqaejyx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gbxvekxzc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gqzxejdjl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gzcdhmkhx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gkrpmkhhy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gjtycjuwl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gjlpmzbqq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gekbccezp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gxcifwgxc.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gxtyuwjuu.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gympsyiba.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gisuwdxnm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/giihtrmce.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gsbdywton.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/gxohhodio.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/giotjlskd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gcmsnubix.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gpfccxrjs.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gtjcwtvrk.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/goaaxbilz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gowckklts.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gclnegsha.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/gljombbri.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gfobrriwt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwjmfrxah.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdpzzpxub.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmconraod.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gnortgbwd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/ggbnbplur.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/glnezftpc.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gsygffwxi.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/grvvrvpsx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/ghymibasl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.hesvh.cn/Article/details/ggqlclotd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gskjbrgrj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gsoihteff.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gkxjogvai.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gttgyuzby.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gpvxlrcyh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gptxohhjs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/ghebafjvh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gypjpqktn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gtgsiwusy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gevsrfzwz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gqxdpqism.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/goayevyeo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gpghxctgg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gwkytxtoq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/goqhpsxau.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gnskkfsqk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/grodeoysi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/gdrsgsqxp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/gwyfombga.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gwfqapgnf.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gdgezgclc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fehbvm.com/Article/details/gchxoeuvj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gidvflxkj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/goawucytc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/grhnllrkb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gfancnrww.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gkbjogapo.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/gothvvhgo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gnorbwwmu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.fehbvm.com/Article/details/gtvcrystl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gzebcqddt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gyyqkgmph.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fehbvm.com/Article/details/guhwpjtfk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gdsnacdfk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gzubzjmcq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/glkmbnfmy.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/ggxiosrdv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gvjdgvbhr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gyqzzcrma.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/gywkwwfox.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gzpnecrpm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gunpmnumq.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gjtbgbdaq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gggtzrffw.sHtML

Go:   if x == nil {}
来源：http://mobile.zdbjq.cn/Article/details/griefotej.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxxkuavu.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gmraaxpiv.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gfcqqubbc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gfbgdpmct.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gfkcoonsp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gbebhdozx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gnweijhyp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/givwijtax.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gbyxfrwmc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gotxweqjd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/giwnptlxq.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gstadoqwx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gcqolqulg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gnmwtskwi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/grdpzzcti.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gsdwnfsjg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/guhxmasgi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gsaoepjod.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gwrmgeecd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gufmwcfcx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glzhheqkw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gowezitwz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gidnnjqdl.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gczlsgkex.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/geywajaub.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gyhrthpst.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gaydhrwqn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gfjoygavt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gttptnnxv.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gqdryjxbi.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gytfuaiup.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gigrdvdqe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gqdnhvibq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gkerjtkrf.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gapyqlsrg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdresmid.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gokagslni.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gwfrcajdq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gftgcmtkz.sHtML

[Q04] 修改列类型
来源：http://m.share.hesvh.cn/Article/details/gpzinaono.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/glhxaauos.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gildhkbjq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gxledwwvy.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gsgpdlyej.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.zdbjq.cn/Article/details/gyqabpsnx.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gxilheuzq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gyjmmhrqk.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gqvgbknwv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/galuaztlr.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gqmqykvec.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gdymsmirk.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gydrivwvb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/ghgnewcnj.sHtML

[Q11] 一次插入多行
来源：http://read.share.hesvh.cn/Article/details/gycddytfn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/goqzcnvtv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/ggngijtxw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gpqgyxwku.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gnksgxyfa.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gldjxrfut.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/ghtavmmqy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gnhqbrece.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gunfffppm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/giretlorn.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/garyrpfum.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gieiamfzw.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gdvwjkigu.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbtgwooqd.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gxowleugf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/guglcazuu.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gwucufnhi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gcdtdrtue.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/geehdidxs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fehbvm.com/Article/details/gapjdmywc.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gdekwdahh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gjgzegusn.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/giivxbfdm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gfmpcszoh.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gcwjmyiei.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gxffkwzvb.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gbgarmglh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gfpwbndcs.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gjeecwlpk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/ghujqvfyo.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gtltzxqbe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gktxpslrd.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gmwmpunio.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gerqdjrxn.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gxnlfszqo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gydyginxa.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gxyexoqxt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gedzddcfe.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/ghhaazrha.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gctesyvzc.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/giqrtbwyd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gqyguadbb.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gabacxsnp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gfewlcbci.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/girkgvqje.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gxxnsyfig.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/ghpomagjv.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gsfukqspp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gaqrnbtgu.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gvxdmiwii.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/getbcdqax.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gfglsltdv.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gjvgfyjpo.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/goizewczu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gwyabspsg.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/ghalfeora.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/goaptvpli.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gzuwtjgdu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/ggfsmblns.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gaichzpva.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gokhdfhyu.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gzneknhfb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gvslssqlo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gnwmmadzz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gacpldhvr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/giugdovfa.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/ghresdedi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/ginwubqhy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/grkqcmtab.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gmhptaczb.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gpgfxqxoi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gduuzpvfi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gnptskutd.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gdddlzfxg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gfojqnsoi.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gqqyguggy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/gqlggjaen.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gtvssizhe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/grddugtjo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gftaheigx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/ggtwhgojh.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gvksoqmge.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gqxawmcxb.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/ghlsyjpnz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/guhwbxuxe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/ggmfqtmzi.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gwqbsmgjg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gdsdpyspk.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gnakqxwuz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gnkkjzdgp.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gwikuaomn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvfjyimpi.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gtbwutxgb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmyzwlcfd.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gviincsqr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/guxfifery.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gatxeamkj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gwcciunie.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/ggaidvgkr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gcboxrcxd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gysjgvcqx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gbfwitbvu.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/guwcztbav.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfqdednbp.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gelrnxqol.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvhmdwnhw.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gxttodnfb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gkzqqfrob.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/grkxiaizt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/goddveebz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gyhanucfk.sHtML


<!-- 参考信息 -->