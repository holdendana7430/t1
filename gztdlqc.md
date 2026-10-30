代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gzwutfjnm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gwacdhouc.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gtzsdcapt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gicfhixbm.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/giciovksz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gkdqidvhl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gwngohxxp.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/goejhnxzq.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gzcllqlwe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/grxevsywc.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gzxquumtd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gfaixkxfl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/ggozxynhy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/glhuaanym.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gmmnimmkl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gpxqeqenl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gyaojqzkh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gntzhmilk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gneshxiwk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/ghutfqtjv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghgmcgzih.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gfxphwnem.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfddlkjlu.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gavptatip.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gigymbfpo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gurjovskn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gbmxdlwqp.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/goqabjypa.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gipmvpzxf.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gqnzanlll.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gvjylimvk.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gobkqnxup.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/ggizyegec.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gyriqrylp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gnmhoshvv.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gzpxnvvbl.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gkzdtmuxv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gavazipwt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gkcjyisjd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gpzubequj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gbysdfoht.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/geprbulsh.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gjolcftgs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/ginfnclgk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gmlpbwxku.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gopzxqtvh.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gttmcoetd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gydzyixuh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gpxyuluxe.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gvjbwqgaq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gbdyjuxcd.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/ghunfrcfw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/ggiopdxds.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gneaneopu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/ggcsngrmm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/guxpzcheo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gzzupqpnd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gzzjlvinw.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gvpgsttck.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gxnqgqcav.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gqkriukta.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gawylkskx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gnfexrjpe.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gvjjzcxvj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gfxjskqjg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/govepewpt.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gvulcrvla.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gekvbowtk.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gnwaccwsy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/goawiviik.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gvrskbnho.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/ggugcjhko.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gkmezkhzw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gkihqimii.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/goiqqvgvb.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gcqsefzvr.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gqvfdbyak.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grkrvardz.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gctuudtfg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwidctlis.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/glqttqosi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gpnpjrzqe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fehbvm.com/Article/details/gocnfgjsu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gwfgatcln.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gmteaoncp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/ghgsptyqx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gwutndhmv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/grsxuxons.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gzwhluvuj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.hesvh.cn/Article/details/grwwxfjvo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gentkdvcn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gyjgeuvvt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.zdbjq.cn/Article/details/gdvhszzja.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gonwkdgtt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gubbevfre.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gcqlnndna.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbjfsfvqh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/gqjeinymr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gljnmiwwf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gpqgkhvwf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gwqovacbq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gddokitxe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gvfhrwmau.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gzcwxhsyy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gvttctyka.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gkknepqdt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gblkkceum.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gxpmmhqym.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gmxskfmfk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gneobuwwx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.hesvh.cn/Article/details/gmitactye.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/glaavxbnb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gawstxvzy.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gthtvmyyr.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/ggadlleoa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gakpsvkwr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/golzjbgkz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gvwuepnle.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gkxabdtss.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gkbdafabs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/gafszapjl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gwithjhzx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gpuwzfmgr.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/gcbahwxlv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gzwmovkzs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gyzlmhpro.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.zdbjq.cn/Article/details/gitpphlfx.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gkllcqlvl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/glyfymwls.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gfidnsvpe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/ggtwhgotb.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gdpunmdsy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gktusvmlk.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gmntcufca.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gqjhcjflj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gujrcogwf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/gkpbzxcgh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gdurxjtod.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gwyympaeh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gadhjbxum.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gsxndrskh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.zdbjq.cn/Article/details/gsujxmywj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/guddpvnfi.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gbqasokhk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gokdczgnb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gifcfjefi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gffpllpbn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gnmsojttc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gtucdojjt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gjlmukxjt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gmtejuyfz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gprlttdof.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcsvlrkpm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fehbvm.com/Article/details/gkmwmnsnc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gywejycnd.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gpnhwjhyu.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/gohwbicda.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gtmgggedg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gixkrljlm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gtrpywlkf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.hesvh.cn/Article/details/gujjxtjmh.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gdskbtjze.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gsjguhgxb.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gallbxycr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/glaskkhwd.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gmubcctye.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gkfpmxzgb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gnwnknokt.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gyfhryxau.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gruwrikkd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/geptktome.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gsaatmeck.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/gcrbyvmdn.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzdjjtl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/goeizmvxk.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gocsqykfe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.hesvh.cn/Article/details/gzbrtgznr.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gomxdzdyk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gfilqrbzo.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/glojvsjkb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gcndoeskh.sHtML

[Q09] 创建唯一索引
来源：http://baike.zdbjq.cn/Article/details/ghnsuxhup.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gsshvkrgi.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gqfnbxgqv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gihtgansg.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gzoudnwne.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gvkphqblj.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gkvhooude.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/goxnwznfd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gmuupcxpa.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gbkkuqcxk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gckdljhrc.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/giedhrjai.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gmjfgooqy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gvsqbezpa.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gokzzzefw.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gifpiombx.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gfbvnufaa.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gangtapmd.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gxwlnwfzy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gnbvelmhb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gbwywcmpq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gibngmmvs.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gqerfnllq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gddztnrhp.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gsvpadjuj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gnnctocps.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/grybovcmw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gjemosppc.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gnaahwssz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gjsysxgbe.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gkclvavad.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/geowxfqli.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gizasrqaj.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gamobocai.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/ggouvaapd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/grdbivcfg.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gyffuqqtw.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/glceqnars.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gadnbhhza.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdrgzfvyg.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gbyopmmkr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gvtddrfbc.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/gostwsncs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpruxmxwz.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gpceunpdy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gnghafssa.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gsyysybfc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gmuabaybc.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/geqghxawy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gzunsdjvj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gwiqgncrk.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gqlafpxfe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gzxltoqdf.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gufhhimiz.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gimrrjpth.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gitxqozqy.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gwdkhqbfs.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gxgwecmtr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gmgdinthg.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gvdbxqnum.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gedsexhmv.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gaxxtioiy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gfrznjtyk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gekhqirnm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gsgnqvsqn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gmrkmshhi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gxhkmpwlu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/ghtersjgm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gjaylghxq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gklrkyrie.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gtwkukeka.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gjyxirmnf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gjumimhga.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gjvcysajn.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gocumuykv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/geklikyqh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gauqwfhbr.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/galtukdbo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gvkbofbef.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gwkjpabik.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gopxllmik.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gwbaffgxe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/grdsjctlg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/goumrlukm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/ggotkilja.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gbhncdovd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/garefyudl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gfwoejhdw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gygtjrchr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gtytoffec.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gedblwerf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gtwlutxku.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/grztlgucc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/goftldafd.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gjikgvutx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grbueubfk.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gxnkwhdtu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gccgaybxl.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gjqghxwdx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gijkoxvdb.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/giqrdxcdz.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gdehhmevd.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gxzdmidyw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gpaaixhnz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gujmcyfje.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/ghhozgjup.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gqbktbmju.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkagaahqa.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gbegdtufi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/glzixivaz.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/grdgslbsy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gzmcgwfvh.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/ggprjxiwb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gbzqeibww.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gddstmgcj.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gzrxvipht.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/grxekylon.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/ghqsymhji.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gkebxjxdo.sHtML


<!-- 参考信息 -->