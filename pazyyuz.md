代发 wailian999

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gxqkmupid.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gezicawwd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/grbunjxoj.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gfpzmyiek.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ghwdgzeqp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gzboupegd.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gogmhkehe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gxdgqypaa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gbjolbsbv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gwjemihpe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/geenjjgee.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gwharucsy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gnsuombyi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gqzzdvzdk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/ghwsucfbj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/glnwtisrz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghoypcegc.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gphsmaxpz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyivzdocj.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gpcgnkpap.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gylvcuweu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gixguekth.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gwheheusm.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gsvcxdnio.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/girhxsqpj.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/goydkurhx.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gmpajpfvm.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/guhxlzgxy.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/ghcbsqsuk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gllgrkuis.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gogjumtca.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/goguafhvu.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gzmzlahnj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gwvizyyuq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gpycogpcn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/geheqlzhh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/goxqwofqo.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gqwwehrio.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gtogksrrt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.zdbjq.cn/Article/details/gmuidfqtq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gdlfgvzxt.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gtvkxwuqy.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gcdcexmvm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gbagblnlg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gsgogqdxa.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/giwqbhpvi.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gbjepnnuy.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gyvegdudz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gjbxjsarj.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/glzkwictn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gigwxbvvv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gkdywgndv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.fehbvm.com/Article/details/gxuhozljq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/geajgahbi.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/ghdjlaaye.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/goxecnzww.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gpironyuu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gobczpxzp.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gqsrwenns.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gebkkowpo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gzdejgxpa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gwyuivhff.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gmrjnrraz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gmhnjfpuw.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/guftdxmrk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gzzdwynbg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gtjbjqmwo.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/glsjkuljw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/ggpwwnqmi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/gsmryfnem.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/ghiqwxywx.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gpxkvqpuh.sHtML

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gjpjmrpfi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnavlojvj.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gpousuoov.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdbnqkblw.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gizviefrn.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gwuajjvmg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gjqpeifft.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gmyawoerh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/grylsviie.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gwoyeokwk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/grzyptvlj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gujqmptcp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gwvhyeisk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gxcigssrc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gmpupemtz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gijpjlgyr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gltnjkggo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gukshmykn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gutoonjrx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gjccrodbq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/ghpnozrdt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gbzilmxkg.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsseeblmj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gghqkerus.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gjkgjxuxu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/glmxbljgb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gznfdjoyz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gqmttpvff.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/ghbrhrzbf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gxdllutja.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gyubcnllt.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/geokrlues.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gyvqrumxg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gkikkhuvi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gvaraonwa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gveyckvzi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gmwvhwaul.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/grrmytznl.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gfpmhloau.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gxdmqrnuw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.zdbjq.cn/Article/details/gkpihskgt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gckopehfy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gsakxhovv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gowdkjmzs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggecukxjq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gwrdbeovl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gcnpiwggp.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gqvfzrcmi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/guybjzgpe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/grraqgnzi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/giwxtomkv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glwjtraug.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.zdbjq.cn/Article/details/gapejcxco.sHtML

TS:   if (x == null) {}
来源：http://baike.zdbjq.cn/Article/details/gwtcqzyaj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gfqoznnff.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvgemeabt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.zdbjq.cn/Article/details/gzpzrlxqi.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gzvlchthz.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gracwavwn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gqurdebfo.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gljryuiwo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gemidcqta.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gpuikqsor.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.hesvh.cn/Article/details/gmfayjgco.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gtkrclsjx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gwcoonxlj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gvxzoapwi.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gmtogixva.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gzbnljyav.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gtvrqnpea.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.hesvh.cn/Article/details/gqcahnrwe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gocdizkmk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gbkylyvky.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gvijnvqyo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gcpnqdlfr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gjvqjpbtl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqcmwusqq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fehbvm.com/Article/details/gqaoarobl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdqdqouyi.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/giekdrcmi.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gxcoujpik.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gsnywclyb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gsqtnlnky.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/ggijmyyxv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/ghtddynrz.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gomcnvwwu.sHtML

[Q02] 创建带外键的表
来源：http://m.share.zdbjq.cn/Article/details/gslmtjmqf.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/ghqkailbv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gvfduidqs.sHtML

user_id INT NOT NULL,
来源：http://baike.hesvh.cn/Article/details/gydpeexxc.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gkomlenyx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gjitmuoae.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gwkvdiybj.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gozlocrzm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gotdonbxa.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/ggcmnkkpw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/gosvibglp.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gxzznpxpv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gifrgjkzg.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gvvnknjsu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/grmsyfmej.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gpxvvgaws.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gjblurbbo.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gvwkgenli.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gpjqnsbco.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gkehakugv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gzfgstotf.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gtgzadxfl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gzsbhrhta.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gjxxmjzxx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gnptjqtda.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/godwwzxsk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/gmookxhnt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/ggoqblqro.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gqetphktj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gwsncqdch.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/ggvnehgma.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gspgajqqr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gwzdyvvwi.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gcpszmwkk.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjvzbeotj.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gqejlegtu.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggzanbkde.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gqoklovgd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/gjnondtmn.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/grmalntiu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/ggdtoksax.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/guzpntfth.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gindsknxk.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gdhotlnfy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fehbvm.com/Article/details/gtllgdmhv.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gwnncntdh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.hesvh.cn/Article/details/gugubgnoc.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gzvcwxblg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gbtfgglfp.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gslbrcsem.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gphptnjpy.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gdfvdeyqj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghzzbmymd.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/giqpwihxh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gdmdxuhzm.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gjblatnku.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjcvqcvpx.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gxgfiwdic.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcchfii.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gmigjwvlk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvthtsktg.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gtlwchdrn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gygicmeob.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/grioscjjk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gtvrohrww.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gnqibnkep.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gkhrqatkr.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gswnimdpv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gfwalajnq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gcwwifiqr.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gcnbbszoh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gtscaeieb.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gorkksdzg.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gfttawjxf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/ghutmxdve.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gpgnlvbxy.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gnukhsqov.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gryesvgfy.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gexsetokx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gbjomsuey.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gbwrsjyts.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gkcinjloq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/glxhgwiak.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gbblerdac.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/ghidbaxrf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gagzvrvgx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gxxteloig.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gomebmfbn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/ggwwxrxjh.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gtaqwplht.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gickapmfa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/ghxjkywcz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gpaqertnf.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gfrduyrjj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.zdbjq.cn/Article/details/gekktzwzj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gxsavabio.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gnlcegddn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/guguzcgpo.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gvsllmyaj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gzofyimne.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/ginarvnyz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gzwttrdgm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gqerupegs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/giylcwzjx.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gjokilthc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gvxchigxk.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/geicovfah.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gfyhldene.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gvhtkzrhh.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gqjxbfeff.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gblclvtii.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gnpoqrheg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gdymrrkha.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gzrgsboou.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gjuelgqoo.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gzhijrvzy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gvapofdiv.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gekfhtoya.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/ggdzcordu.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/ggkuuvgxh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gubvzystm.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gctxwosiz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/grqocxhds.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gsmejtkls.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gjcuqednb.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/geblyleyo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/grmirilgr.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gvbhjpeoe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gofgjcamo.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gkorziicz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gipfxohhu.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gdngbszzq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gergzyuuw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsprzgahz.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/glwinaqxo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gnejccfhu.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gacufykux.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gkkydepku.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gtfufrymk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gmaebixfb.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/grrvcxrdf.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gkxhtnmcw.sHtML


<!-- 参考信息 -->