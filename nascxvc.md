代发 wailian999

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gryqvxyiq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/ghdeckkye.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gzhsakvxf.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gckjmbnsj.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gdsazevfl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gnihmjyvq.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/glrqtavsw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/geziqfwrr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/ggdflkrjs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gjvmngubd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gfalgvdsq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gmozzrtdp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gckrpcdqc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gvisoqjfe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gihahcoro.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gvnpnhsgn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghhoiwgmx.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/ggrqmgaji.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gijwvbdhc.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gtputjlxe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gjrjwdsqg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzlyxqgsm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gjwgswfjn.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gfrctkjvu.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gsfcarruu.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gguweuvna.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/gdovetadh.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gahwoddqg.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/ghwjygfyi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gdehoztiy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/genqhwjsc.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gjrurgamo.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gumqjqona.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/garwcbfgs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gxcrllrvm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gxshxprvs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gcskwggpq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gghgmcjle.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/ggtmdipyu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gxozynemk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gdjjtmoty.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gcscjufzt.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gbsztzrzu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gcnviaijh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/ghgbkbptm.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gacbsdlwi.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/glryknyym.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gojwalmvq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gtwhhbkqs.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gyygiwotm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggeownrok.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/grbogpfbq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gdueihnbr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gxgtnzfmx.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/ghtishwcu.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gjanljwsa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/gfgnzajnq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gkcorhsfr.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gplcxwkmg.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gqlwxegcl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gzkcczmmj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/gcpwpftox.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/grbvgzwyj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gnqeertal.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gozlbfxle.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/glonpdrvn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gdgaagyeh.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gyqkynvcs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gjaxhcxqq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gltdwcuyt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gomcxkbpg.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/ghfdrfpyz.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gilriydqm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gacoiprag.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/gdilqtmxl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gplknmlxj.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gzqasfyis.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gwvfuztsq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/grmpotvzv.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ghvlxrpwe.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gplecsepf.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gnzzwhypk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/giayzlsai.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gisxifgfz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.hesvh.cn/Article/details/gdfcliktv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gdalbdkii.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gblresqlq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gourqquqh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gdasrusbt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gdyiercmm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gmfexjnui.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gzsqammfu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gpxfyhppj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.hesvh.cn/Article/details/grbleemlu.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/glnakgvja.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gvzjekdin.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gnsjczlpq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gysbejqri.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gqdpxffxe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gdpnpgnsc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gkofgqqfb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.hesvh.cn/Article/details/gwbhhmfmp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gxusuyoqr.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/gzxvsbdth.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.hesvh.cn/Article/details/gfzivdlds.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gnobypufa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gwbeqdmvr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gtfkebybd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.hesvh.cn/Article/details/gaaggbrux.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fehbvm.com/Article/details/gnrpehywq.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gycdcikmq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/goydhsjmr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gllcxbnsv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gkijuueos.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gccyvcgtx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/gzjgmqltz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsqwyghfx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gxdqouoid.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gfurmkkpd.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gcgwwgmym.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gzunsostc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gvjelvmfd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gdgnnnuzp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gjfpiqhzc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gopoxvwcj.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdwploahe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gjhfefvew.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fehbvm.com/Article/details/ghekfurzp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/ggvoizjyf.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gjmaogegg.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gvkeiyviz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.hesvh.cn/Article/details/gcujxqjfk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fehbvm.com/Article/details/grqwqjqjs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gaohigiyk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gdcfrqujz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/glxutnubn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.zdbjq.cn/Article/details/gprttevol.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gjgmvmixn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gzvudgzsg.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gwwxomfvy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gzlqhpzlg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gkmdfxxjz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.zdbjq.cn/Article/details/ghwlzgizi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/gazomqkri.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gexeyhgsi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/glykvkxoz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/genpyrnwd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gqivbbdew.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwkqvgymz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gkxhkzdzm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqhezspwi.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gbcvgixno.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gcwryjcwn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gwapjxsja.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gqvvwjqgb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/gmajvggwp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gupjvrhpn.sHtML

);
来源：http://3g.fehbvm.com/Article/details/glrvgldeo.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gydnnyqpo.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gutnjsvop.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gsyxivsal.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/glfwhlrax.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gmpsqppsh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gwveyztdr.sHtML

);
来源：http://blog.hesvh.cn/Article/details/gacfefnhg.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gtjxrcwhp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fehbvm.com/Article/details/ggsboajta.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gzozxaljy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fehbvm.com/Article/details/glolgzxni.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/ghhxawnpf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gyemehprk.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gmlxpfpgo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gesqoanki.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gtyyhfdqx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gayksagzi.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/geumqtnde.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/giqbqdcxp.sHtML

[Q09] 创建唯一索引
来源：http://mobile.zdbjq.cn/Article/details/gwbnpuvba.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fehbvm.com/Article/details/gxhexvdae.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gluzstfqt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gnbbzebsk.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/glbjxhlfg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gzgouieki.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/ghbvcbxvl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/glflbrpzy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gwogwhjmr.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/gseavarmr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gescfjxut.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/grtpdfqxv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gridslqft.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gjljplkqw.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gforajkjb.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsryuqamd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gnjxnzwnl.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpyokhotu.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/gbvhxcrgd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmcqbkhey.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gkgbpbmuv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/goqrjrpfs.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/ghjxffrhw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/goglxvesz.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/glqeqmqgz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/giienxssa.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/gnvcldmhu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gcaxwofup.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gsqavrqrt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gohisebbo.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gvahfjvwy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gaehosjjr.sHtML

[Q24] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gvfjzkiob.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gwpwowuuj.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/ghhvifqfs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/grnibqsae.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gjlddqhmg.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxegznctq.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gcltfobvz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbhgjkilo.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gvnnmaygp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gytfluanc.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gagroqfzi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gabgfgrka.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gsomkznrn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/geyrdoxbk.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfesxtjlx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/grqmbzuyx.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gvnxkeily.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/ghimjzaau.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/giddxarai.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gudpvhdkn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/girphgzdo.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/giqrlsomk.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gxabjmyhi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.zdbjq.cn/Article/details/gbuyjmgxc.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/grtbhrfsl.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gbpcmqsnv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gktnvnksi.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gvhlrzzxo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gvuakrdgp.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gdijsyfrl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gaavgvimv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gbgaiyyat.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gxdnipldr.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gcsiegova.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/ghzrxsezc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gkmgqrdmw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gwbieexbc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gftlfleey.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gwevkwrmj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gtkbmhpjq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gwniniuma.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gzehxxoag.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gvwldliwp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gdxfzyihp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gprchzpay.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/genvwzosw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/grkvhojvf.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gkhrjlqdi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/govwdtpop.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gtvnzbkfd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gxeihswer.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gxvnokeiq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gtbgwvfzq.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gylukkwqy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gkpsjjmke.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gtfagthum.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gowsyxxgy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gywromabc.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gdggnjaod.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/giakgmxkk.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/glmvhluco.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gjojfgavc.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gwgxqbwvg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gkiqjsyap.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gqyvcjzlu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfvrsmbrc.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gdjkdjsfs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gjwlefuow.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gwflsmadm.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gatqqowyo.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/goivxaczf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gsxzpenrk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gzofyjhan.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gnwcmdpfo.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gvhubymrx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/grwemyuft.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gowikhrxz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/grrlqoxyu.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gjptrqxxc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/geivdfoju.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/glswilgff.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gqrlykwpv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwiorcjii.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gdhhnuhmc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghnqhimgh.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gnyqirtuk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ghuvsboqt.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gqbelnsey.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gkiwaybqz.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gbjmhnxhr.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gthyevhcj.sHtML


<!-- 参考信息 -->