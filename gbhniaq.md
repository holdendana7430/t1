代发 wailian999

PHP:  // 手写递归函数
来源：http://wap.fanxiaobao.xyz/Article/details/gutsgzpfz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gqmkqarfz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajwjdhnx.sHtML

Java: // 手写递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwwsqmho.sHtML

Go:   // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gnllsyvds.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gqtjckzft.sHtML

C#:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gabwwnesj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdhgeohd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fanxiaobao.xyz/Article/details/ggdrhjmem.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fanxiaobao.xyz/Article/details/gpxbozqhz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gytrcbjtq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fanxiaobao.xyz/Article/details/goflekrzj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fanxiaobao.xyz/Article/details/gwveoudxz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fanxiaobao.xyz/Article/details/gwaoohqhu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxkkfabp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fanxiaobao.xyz/Article/details/gbtddhtmm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkeegesta.sHtML

O. 并发与异步
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqiiqhn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajgooxwv.sHtML

[O01] 启动一个线程
来源：http://www.share.fanxiaobao.xyz/Article/details/gddzyaatk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtklehoj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxlivbty.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fanxiaobao.xyz/Article/details/gbeaiahsp.sHtML

TS:   // 同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvcpifjo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpxbsdqm.sHtML

Go:   go f()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbhnnolv.sHtML

Ruby: Thread.new { f }
来源：http://wap.fanxiaobao.xyz/Article/details/giojhjgko.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fanxiaobao.xyz/Article/details/gvctskgkj.sHtML

[O02] 使用线程池
来源：http://3g.fanxiaobao.xyz/Article/details/grphzicwt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fanxiaobao.xyz/Article/details/guyzxrpkz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fanxiaobao.xyz/Article/details/grrbmbrpr.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuxkdxqv.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduhmrvda.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzaapqqg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhuefcey.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fanxiaobao.xyz/Article/details/gqcrifaoe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fanxiaobao.xyz/Article/details/gpprwayou.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbykqbvv.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoukppeh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixfiugzj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fanxiaobao.xyz/Article/details/gmorvqkyy.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/goiptnmvq.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/grfjdefxn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gsnlfqawj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/glozlhhfd.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjnmrqocp.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/goraaudbx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fanxiaobao.xyz/Article/details/gughmwoae.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fanxiaobao.xyz/Article/details/glexzzhiz.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gffjnsanh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fanxiaobao.xyz/Article/details/glmqyeyxn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxajowpv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwykpcwi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/gopieywds.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmlftxxwi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyccrefl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktbmnuyx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fanxiaobao.xyz/Article/details/guverddux.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gryvkwdoc.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gubwqqiaq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdhihjbu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fanxiaobao.xyz/Article/details/gmqrperpe.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjyjrjli.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggexfwsnh.sHtML

[O06] 使用进程池
来源：http://www.share.fanxiaobao.xyz/Article/details/grxipxsxo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzrogjim.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqpxjcvl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyetlaqcp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gutfojkls.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fanxiaobao.xyz/Article/details/givlyxveo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fanxiaobao.xyz/Article/details/geqmsexzy.sHtML

Ruby: // fork 块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbytjvck.sHtML

C#:   Parallel.For
来源：http://blog.fanxiaobao.xyz/Article/details/gyzdtikpg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonzltrub.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgqgwvzi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/geefoptuk.sHtML

[P01] 生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkypqxtz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvuzopyl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gwzrjfgou.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/golbuacaq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gkjulgwkp.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gyifmkgnz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmfvfxfr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gzauhzxka.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxysbsmzz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzkddxnb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzfkqyzm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gmtigoicv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fanxiaobao.xyz/Article/details/gcsgxdymq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fanxiaobao.xyz/Article/details/gxfgscmpw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyaqeppy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fanxiaobao.xyz/Article/details/gqxwntwte.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkuvalwj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fanxiaobao.xyz/Article/details/gfautcfcg.sHtML

[P03] 生成短随机字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gaxhcutku.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzzvqgkk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fanxiaobao.xyz/Article/details/gvczjjube.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsfsmohm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfejzbet.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkevhwijy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrdlvacm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoxuribc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnjyeooe.sHtML

[P04] 求长度
来源：http://3g.fanxiaobao.xyz/Article/details/gekjldrva.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fanxiaobao.xyz/Article/details/gslfzcozd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvqwocql.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fanxiaobao.xyz/Article/details/gsifgztvn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fanxiaobao.xyz/Article/details/gbcukjqpt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxogfvbni.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fanxiaobao.xyz/Article/details/gnmaprydo.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweyohorc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gyawmfdtn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fanxiaobao.xyz/Article/details/gwaqegrau.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuelhsvh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fanxiaobao.xyz/Article/details/gkrenkcpw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoygpgsi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsextphvz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fanxiaobao.xyz/Article/details/gigodznzu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fanxiaobao.xyz/Article/details/gqyberhrn.sHtML

Ruby: a == b
来源：http://3g.fanxiaobao.xyz/Article/details/gifxgrwjb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fanxiaobao.xyz/Article/details/ggxeroyhy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdmfzvft.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gkupzanss.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gyapbjown.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfbxsxax.sHtML

TS:   if (x == null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjwulwlog.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcgnepae.sHtML

Go:   if x == nil {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbhkerga.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbfnfwkj.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnqtxjbg.sHtML

[P07] 防抖与节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscazwqhe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fanxiaobao.xyz/Article/details/gozkoncln.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fanxiaobao.xyz/Article/details/gadijjifp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehaqdscj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gaceilcbf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrxbzzzj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fanxiaobao.xyz/Article/details/gzcyhlegb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ghukjoyef.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdhuvgep.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fanxiaobao.xyz/Article/details/gwcmtjoms.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjcfrwyu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhihlvmm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fanxiaobao.xyz/Article/details/gxryqasje.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyctnkzvb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gljrhubrz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxoecuoe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelhybmse.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvyongcw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdzxhcehn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fanxiaobao.xyz/Article/details/gspcitlln.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guiuuldui.sHtML

[Q01] 创建表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmpsittf.sHtML

CREATE TABLE users (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvgolcee.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fanxiaobao.xyz/Article/details/gqdpagrwp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fanxiaobao.xyz/Article/details/gusvogksa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fanxiaobao.xyz/Article/details/gqcnzpyqh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxewlgfr.sHtML

);
来源：http://blog.fanxiaobao.xyz/Article/details/gvzhzkkwm.sHtML

[Q02] 创建带外键的表
来源：http://blog.fanxiaobao.xyz/Article/details/gjeutljzd.sHtML

CREATE TABLE orders (
来源：http://baike.fanxiaobao.xyz/Article/details/grlzrfbsi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fanxiaobao.xyz/Article/details/gcjgxnhxp.sHtML

user_id INT NOT NULL,
来源：http://mobile.fanxiaobao.xyz/Article/details/gplwyucvb.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fanxiaobao.xyz/Article/details/guqhjdtyf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fanxiaobao.xyz/Article/details/gcmlvfzmm.sHtML

);
来源：http://wap.fanxiaobao.xyz/Article/details/gxlodmlri.sHtML

[Q03] 增加列
来源：http://read.share.fanxiaobao.xyz/Article/details/gasfydufl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gddmycasg.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gkalqfwxk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gurqmrxeh.sHtML

[Q05] 重命名列
来源：http://3g.fanxiaobao.xyz/Article/details/gnxtrnkbg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fanxiaobao.xyz/Article/details/gmmwkknrw.sHtML

[Q06] 删除列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvablmkzz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fanxiaobao.xyz/Article/details/guryzkdxf.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/ghkchwtfy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gxahdidlc.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gnewjhsqy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/grqkgrgqd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmdgwdft.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fanxiaobao.xyz/Article/details/gexfniwyh.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztvisdvc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gncbunlqz.sHtML

[Q11] 一次插入多行
来源：http://m.share.fanxiaobao.xyz/Article/details/gntqpdrdb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcweresk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokiazwil.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fanxiaobao.xyz/Article/details/gbxsxnxpk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsmpmhpy.sHtML

[Q13] 忽略重复插入
来源：http://blog.fanxiaobao.xyz/Article/details/ggghyuchp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gfayvzrrv.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/glzkksfet.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gscnfxhth.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fanxiaobao.xyz/Article/details/glrlamngo.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbtlyfgv.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbelcnao.sHtML

[Q16] 查询指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gauklnian.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guqassrhz.sHtML

[Q17] 条件查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gjepywqzd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzywucsgj.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gshlrdbew.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gmsqoullz.sHtML

[Q19] 范围查询
来源：http://blog.fanxiaobao.xyz/Article/details/gonwpbqtu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/glhorktoo.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/ghbuvvxmq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzyhitlt.sHtML

[Q21] 空值判断
来源：http://mobile.fanxiaobao.xyz/Article/details/glrtqjqwd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fanxiaobao.xyz/Article/details/gsdeckhra.sHtML

[Q22] 排序
来源：http://baike.fanxiaobao.xyz/Article/details/gudhuydnc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwqinolh.sHtML

[Q23] 分页
来源：http://3g.fanxiaobao.xyz/Article/details/gpqyshyug.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrgfsctm.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gpmpnikdl.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpdzcyhjy.sHtML

[Q25] 只取前 N 条
来源：http://3g.fanxiaobao.xyz/Article/details/geklnkrdu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gxnmgjbtl.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gdfrpfelb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfoydjds.sHtML

[Q27] 条件计数
来源：http://3g.fanxiaobao.xyz/Article/details/gfouklfqi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghefcgmze.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfjynxgb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrucbnov.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gtdwygfso.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjoqiqdn.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gsielxkjs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/glkxsevpo.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/grraqllve.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbsunrgf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkoedhjd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gxnnkuyqy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fanxiaobao.xyz/Article/details/gthyfuhrp.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/ghnhlvozc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghscogyix.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gseuoeryi.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajlbaigr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbtpbpkn.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gwiaxqbdu.sHtML

[Q35] 内连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezbpgdmy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkpjdyaq.sHtML

[Q36] 左连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstrytjmr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/ggkdnegqc.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gfkziuerg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhlshglb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/goahmcnnw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvikkwzk.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlfgogri.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fanxiaobao.xyz/Article/details/gcuuhjwdu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gswnwuuwe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/ggwxnjqwe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gawwydtki.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/gunuphcwi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gbofpgxbu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawjqbioz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsysgbpxy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/grswcttfw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqysnzmiy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyhqxgyc.sHtML

[Q43] 标量子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gdejxwens.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gosfsuqtl.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gxygjvnzl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/grknqqszs.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gyzbgwjai.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gnabplxjr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/grvtiqzeh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gepqgfjfh.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gojytottn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/ghrqfqtyd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaqvjiqs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gijavzlfj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/garbvskuq.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxueyhvek.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gajqmmgan.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/gwmukiynp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyznimhij.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gawxzxahv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdubxqnh.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxxjbwez.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gwrihfkur.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gqpdmpgjq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdrdeuvd.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxeiuuwb.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gvxlnamzm.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gyrqauwuo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/goomykgtu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiadhzbr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfkuthox.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvakazbl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/guphbskwd.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gscvadvmq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ggphlhvti.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnxrcxpc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grevjzbkw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gywdxhqxw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/grvubmsdt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gpdhxggzk.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gynoduunc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/grzzfyima.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/guvnwxwhs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwqaahcs.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/gzushrmow.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gizqeneol.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gjtmvhjcy.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/giekhbyfg.sHtML


<!-- 参考信息 -->