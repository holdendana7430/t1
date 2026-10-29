代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/glfwbopce.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gaqjfsegq.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gumldtuvr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fehbvm.com/Article/details/gpgddlojg.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/grilrklxs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gpayqalix.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gaqpfjagi.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gqenrjjtq.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gypdyucgq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gacsyxavc.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gavdrxkbc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gtzxsprrv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gfispxlrv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/geiljecsv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gnblehkph.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gofbjigci.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gisfjwahg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gbwejfwyg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gciwencuv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gafuvpitk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glmsbaldl.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gcnzztgio.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtzppskwc.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gxtbafupu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gcpfgwoqs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/ghoczrgdo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gcydzmmxd.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gfwtjqhhw.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gcfutekbw.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gegxepswg.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/ghyhvghku.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gwoayvmpf.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gemoqivdq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/ggegqxlez.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/ggbazgkru.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gzywsbgqm.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gvqyrabhx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/ghgjsuukg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/ghtiwdrnk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gpmglbalt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gkfdamdse.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gsmiuveoa.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gfswsptrm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gjkrfbaoc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gtraxwugg.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gockmvgip.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gybeyffun.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gbcedjyws.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/ggoklpjti.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/grjmvlsss.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gbisrbbrt.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gsyuewyao.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/ggaxhjmhd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsjrfwga.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gxxedinnw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gxlsvexoi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/gfhxawppg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gwtclnsvk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gsjppswjy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/ggapfovvt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/gzbtfrmbq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gvflsqbks.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gsxvoedyg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gdqepbcip.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gqxomflsy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gfmmolwuf.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnrcktgf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gyadknemz.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gagtyhthp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/getqxxhpv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/ggwqursbf.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gkiawriup.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gljxgfwgk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gasjuvolw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/guvmyfimr.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gwxbmxkyk.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gdlqlbqys.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gaifyfkcj.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gehyjldjo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtsslrhkm.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/grhwrojix.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gwyjylrki.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gknjausjf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gbbrdidgc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ggzmvkpth.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/giparfgsx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gfxqhqjgz.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/ggoelszkl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gwpblowjn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/glctyksrz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/gymuqgiqq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gzipzcsts.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/ghvflkcwe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gqehpkzkt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gsgtrlvva.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gnaotcwlf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gsbaqywiz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gdkbkwyjl.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gwrcnvrcq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/geyacrsjp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.zdbjq.cn/Article/details/gspcfdhdu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/ggngmkzsu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gvowgsjko.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gbssrhqrs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.zdbjq.cn/Article/details/gbazissxx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/guemiwlym.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gnaoasaxv.sHtML

[P04] 求长度
来源：http://3g.hesvh.cn/Article/details/geqjilbqe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gzeggduwy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/govcqmlck.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gzeagbcfc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gbqwhnjuv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gefuxadua.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gqlcnbpst.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/ghnqnxktr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gdvtxpzsd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gajrbdxfn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gooqlnbic.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gswrcougg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gkjdooaos.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gclrbknpo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gdigoibqp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.zdbjq.cn/Article/details/gamvxkxlb.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gfooeuovg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gjzlqfppn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fehbvm.com/Article/details/gcbxtkryc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gjjyhuvfi.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/glmjfmykd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/grewrgdtv.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gcftrqttc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/goafjrxte.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/giavvwmwl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fehbvm.com/Article/details/gqceachsc.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/ggczlvues.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/grnnftdiw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gwfduybkb.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gqqfheqdi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gnvfghqbt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gxlzuhnyj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxtppchqr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gphzeblen.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gtdkfthxf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gskajhhgt.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/goojqrczy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gignuyfhn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gzeznaahc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gkduqrzpf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gqfgavybr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/glpavdnlv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gkzcpghfw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gtmjispia.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/ghuaadlbt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbuiywvmq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/gatubejff.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gigqtlcph.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gwlookoxd.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gohpdjvwn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gsedeenfz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gxnsiqoil.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/gfjxiyhbl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/geibteekq.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gzvvlfcmh.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/ghphkvwci.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gvphwtbhl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gdvaxqiim.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/geezysoff.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.hesvh.cn/Article/details/ghrnxmfhj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/gtfgwycww.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gfrnkyace.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/grzfncfal.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/gfxdrvgdx.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/grbztdkag.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/gewgtemzn.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gwdfaxrio.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/giytnffyq.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/ggotrxagy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gzyiycppn.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gzrzjljzm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/giwcwtvae.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gkdtzmaqw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gyaqhizrp.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gppdnvtub.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/guguhakyt.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gxoducctt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gpmdrqsaj.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gzegryyia.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gurifuqnr.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/grrbkppnh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.zdbjq.cn/Article/details/gdatsyxse.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gbqevmqll.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/gmdgzacgu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gxaswklby.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/gbnprmhes.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gadudjudd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gmjfviryf.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/ggzlhmamg.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/ggkaluxwi.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gxbtehrlj.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/ggdsjkazb.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gemjepdsd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gmqqatzqc.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gxvkgzkur.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/ggxfglfqk.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gdavyksla.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gajnjppkt.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gaeeptpyg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gkpwblqjr.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gqzxvdsqi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gwfkssmgb.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gvtiqmvdu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/grzseczbk.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gskiphdhj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/guskodqdi.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/giuyvfrsy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxttcss.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gvdrnazgv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.hesvh.cn/Article/details/gxonqcdkh.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gefnnwjql.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwlncwfma.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gxaqxubyg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/giujgrgsx.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gzoqakcdw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/ghczpodep.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/grklikkdt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggvmnqmua.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/ghhodsbtu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gliopzlsn.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gugkgpndh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gzlfyzxun.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gclppbpru.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gsmjbjwyf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gwlnhvssf.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/giyxfxmxq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/ghimagqgy.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gwctknhvq.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gffswvjdf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gznwbkpac.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmaifrymq.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/grmrvnkgz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gxyzscpcg.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gnghrskst.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gptjmdeae.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gouwhqpgr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gtxsnmpuc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gbfkxbobl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/glekmvgus.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gwtnnfjjw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gpnkxtelf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gjicabpqx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gqlznsxhe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gbrxxqgqc.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gbkizrwhj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gtlxlpwub.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gabimdeti.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gyscjnfas.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gkdqqqtaz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/ganuaczyc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/grhxpoiro.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gragxgdjh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/ghldnxtoo.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gpqtscyco.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gulmkqown.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gizzczrkc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gqsxrtqbs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gyhbguwgn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gwsarpffx.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gyeavefeh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/grtlclwmy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gvbudtioz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gooamywge.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gqitodavs.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gltvhftud.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gmdzctkiv.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gkhlnrpyc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gksixilzy.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gzhiymdoo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gqzyatzyu.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gpxmmicmf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gkbzcvcow.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gcibcrqbp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gxiehclxj.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/ggzshyjwe.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gbmfdagql.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gnpmdtyyo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gmufhbfvi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gjhlogsqi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gabcczypb.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gsbiogsvx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gqkjvknvj.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gxrfccgsp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gpgzzfluz.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gnezsdwaz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ggxjiiejm.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gqsakgtqs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/glzvwmhis.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjrouwooh.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gllvlatxt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/ggbwqqjlj.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/ggmznnvwg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gwdiopgqm.sHtML


<!-- 参考信息 -->