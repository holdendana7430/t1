代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fehbvm.com/Article/details/gwlzxhpmk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gfnxfwtmu.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gfvajnmpw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/ghcrosrgh.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gpaclkphe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnysgzfwm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gkntndego.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gishndnkj.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gsriaanfg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gxhfsnrlz.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gbkgejted.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gonmcjrdu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gljnfrrnp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/gxamoahlt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gekxzxyab.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/guqtoaeao.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gmwcdyxhq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gnknxsluh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gvvtafihz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ghoiipssl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gndvxmpoo.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gkmoqzewr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzmuxlbvx.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gajtxgbie.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gztyatuzq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/grdzwcjil.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gyvgwmdpz.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/geijqsbfn.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gfmulvipi.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gsvvqjhhk.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gbknpmvfa.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gbhflzlmu.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gvoyhqcmc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/ghjuitijk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/glcrqlqgd.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/giscnabvc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gdfkahgol.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gongonieu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gxjmqomvq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gzrnjlwzs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/geyruoqld.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/ghknrfuip.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gspzzvohg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gnecknvbt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gkhyiyqtl.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gnjjpfslu.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gmrzbufkn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gkvagrozo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gdykokxou.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gdkhmqwrr.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gvbyodydp.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gnvnhfdlh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gufgnoruh.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzxdbqngx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gedjxvjqc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/goutgepib.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gmkhrfzry.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/glrdxpbkm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gmvooalcj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gtzgpoxwj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/guqgoowsu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gntrkgtvq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gmskwbrbv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/guairhcqr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/gxzzdjgeb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/giavoptgc.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/glfzyjkdk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gqewfcaxa.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gcnlidmkr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/ghcntebyj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gchkfdvuk.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/grtdwhryw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gciqmhivo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gcnzaohgq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gpgsjlrmo.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gthhmbkrp.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gfblkqvsn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkjyanydj.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gczskrhth.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjjbftpyn.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/grfovqhyd.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gduunlbsw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gsbsjtrei.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gfxwzbocp.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gjmmnuahd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.zdbjq.cn/Article/details/goqucmscv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/geewreqil.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gzpczwtgs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gzixwevsi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gdsnssrfx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gzzjxmenh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gnqoqetll.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gsyqfrlji.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gfqzifeam.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/glscbahwh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gqoinqgil.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gjqabhnix.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fehbvm.com/Article/details/glyjdiqdd.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gxfymbwzl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gvllibkgc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gfvgvnyba.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/glkmadzwi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/ghvtrppkk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gbrzcxawk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gnbwcxubq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gulwollsa.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.hesvh.cn/Article/details/glhvoeboy.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gbhphwuou.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/geyaclpso.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gljzceyea.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gbarjwnfe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gnwkxiafu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gwudwxyhe.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gsntiafld.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/goklxssrv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/gwgkawuqe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gfhroduqm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gzemtsuaa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gnciigunv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fehbvm.com/Article/details/gytckfukf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gxhtryfsb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/graajbxgx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gxkqfnlih.sHtML

Ruby: a == b
来源：http://m.share.fehbvm.com/Article/details/gzhpolbvu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.hesvh.cn/Article/details/gtoeyuyrq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.zdbjq.cn/Article/details/gwwmjvskl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/gagqccfbp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnxhsllnj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gpaztdjfd.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/guvjshuqn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyajrmeft.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gqtrnibku.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.hesvh.cn/Article/details/ghhovezyi.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/ghnvlfant.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gwijuccuu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gywkirina.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gtnvfwdfy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gtjmclirz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gseqliqor.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/guwuvcjja.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gpxbxbsgh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.hesvh.cn/Article/details/goigfmlxl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.zdbjq.cn/Article/details/geecimduf.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.hesvh.cn/Article/details/ghztzggqk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fehbvm.com/Article/details/giykkdfwm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyrrxxdwb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/geoeucork.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gjmnshbkm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gvtprkeys.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gejhncbbx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gsxussdjy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gbbjdfqho.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/galdszgoq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gyzmlkyfp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghrzrjkdr.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/ghfkzhvgu.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/ghfmssjis.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/grweyakpi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gagbxhuch.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gpfsfgabd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gflbzermu.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gyicmgbba.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/ggkgvlvfl.sHtML

CREATE TABLE orders (
来源：http://www.blog.zdbjq.cn/Article/details/gxweathdk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/gzbocphdz.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gichyufjf.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.hesvh.cn/Article/details/gozvqnlmv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gyiiabumz.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gjhyfkmdq.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gicsklawj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gnsxymyna.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gqlyoxltx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/gygvfkzet.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/ggokezrwg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gxazehcmh.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gjkwecnxm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gmvvmslkc.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gyydsviwo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/gbivlljex.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gmdlfnyea.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gjydxadwk.sHtML

[Q09] 创建唯一索引
来源：http://www.share.zdbjq.cn/Article/details/gvijrmluf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gpepgtvne.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gujauquyo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gmwuugira.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gmybuonog.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gzcgmvmqj.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/gjmmpmape.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gqivxfllb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gldizfbbc.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/getqtzmdc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/geianujkv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gdajuiuam.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/guxgfmdjb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gjrgzkqbv.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gcuztkijg.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gfdpgkaxx.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gvtvmyqmw.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcwovvaqt.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/gweekgqmd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gsvgynfmt.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gvymikzzq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gxhuspvja.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gxxrysnze.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/ggcoispfy.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gmmtbdwfn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gzxsrzelm.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gzzcgiccq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gcidwqesu.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gbdoaauhf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gdmgtyxix.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gvdevnzcv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gwcprjxxt.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/ghitqyguk.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdoqsratd.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fehbvm.com/Article/details/gggecaevp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvqjbhp.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gdqvviaem.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwttwkndf.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gdxlxflak.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdjextkul.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gojhiemlc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ggbjbisnu.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gcinrxujs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcxqfzelo.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gxedemeaz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/glltshhcr.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/glgndklum.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gjspedhlh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/geggkjdfy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gyosibjqq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gnaghsadt.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gopfsyjvq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gjqyirotq.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gruasfhku.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gavwyekao.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/grzhxvegf.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/glnjvsmrk.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gwypjaage.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gcnksiaoj.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gaqqqaubc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gomwjkfjr.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gjqnfrwli.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gdrbwnefc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gmytqmnrd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/grxwfleqb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/grdusssjw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gufjpvqfa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gqqzzolcc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gepetnswt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/guvocglhv.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gejvawghk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gsdwcknbt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gguxftobu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gwzrrwtqx.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gmwpuphcn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/guvmznxqx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gbvgprqrs.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gzdtswcba.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gqskvnaik.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gwqhotpir.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gfxlzjhuv.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gfjyyhjcx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/grtnxosxg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/ggsmskdkx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/ghphvvwgb.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gtjyojmyz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gnhfizdvy.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gmmleuqqh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gntbjdraf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gprffvlsm.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/grzulzats.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gfztdyloa.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/gtknwjlwm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gfojyksoo.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gozboxysz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gasaixqqh.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gvlsbwshz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/goyjygekm.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gvemeofnl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/glvokooyo.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gveiyehsl.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gnrdpetbd.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gmnaqbsik.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gmeguofaw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.zdbjq.cn/Article/details/gloywofqn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gvwwrxmcu.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gbrceigcr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glsybpedb.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gkotixkrb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gwiaehiza.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/geaylcvbg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gipmkayfo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gtezuitzu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gievbfxgo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gmhylwspk.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gdnzwfktq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gjsyxdivu.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gaiiolumy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gthrftfek.sHtML


<!-- 参考信息 -->