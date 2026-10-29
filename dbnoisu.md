代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/ggeazffsg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gltzenkhp.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gvbgaspsf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/ghnlscpyy.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gnrrnvcmn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gstzvlzld.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gkgkcpdyp.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/guanaxmsg.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gwcvmhezw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gqjmodqmt.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/ghazxnlit.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gweopzppp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gvdssyyye.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gwtnbmewi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/guaoqtpxo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gasaiulbs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gkupyeqrl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gvdaprdnz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gppzitmkd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gmisqrrxo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdgwzjxrt.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gyyegbwod.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjyauidhc.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gahqnozms.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/guefltusw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/goonwgdof.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/govznlleg.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/glgowukqb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gdemwsnpa.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/goikuplxx.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gqhucvbta.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gxgnoujjk.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/guqwfxfqr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gnpzicqri.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gpifinuzb.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gysdwplpi.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ggqgogqaz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gqdnwdtsh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/glznsmtlb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gkkihomqd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gdnwbrtcl.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gekjvazfk.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gsqoyovii.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/glswfqeid.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gfsllpbdg.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gqiaoxwbq.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gnvqjznet.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gmfyhvyrk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.hesvh.cn/Article/details/gsfpbrnfu.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gkgcsdcnq.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gyjpijnam.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gyjbcclxr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gwqgxfcor.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gktrovrwg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gteroiaqv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/getczisqb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/geoxdgizu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/ghrrrnged.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/ghuekvlxf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gkxzgobfm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gbfkuepio.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gpbcqykhu.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/goxvijspz.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/ggodmwvvb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gdiqcrurm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gqndylpgb.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gvkecodxi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gfkvcbftl.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/greqmomnd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gvrhyujeb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gjooapkvt.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gdfjgpwme.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gxaqdkszr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gajadlrrh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/gqqfmyxdi.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gqaqrcmkn.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gbrknvmab.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtjlzzkre.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gtbkihasc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmnfftozm.sHtML

[P01] 生成 UUID
来源：http://blog.fehbvm.com/Article/details/gbrmvlwoq.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gghyosvtt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gzqekoply.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gozxwuwee.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/goghxtavi.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/guausgtjq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gibepbvqe.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gisqxksct.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gbrqguold.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gvaeqfobj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gssomhhkq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gjzugkbeu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gyggucdio.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/grkxilwou.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/ghfokxozs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/ggyimjphn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gqwrshxld.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gzggzmbzf.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/grufpfjxa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gjkdxtive.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gaibwufup.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtgfuvmzq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gobrjimjj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gzawczvrd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gxqrdeqvo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/glgyhurri.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gzmnjhmkt.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gzqjlphvy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/ggqwzywbc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/glgocaarj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gildkfltn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gjsihxqkv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fehbvm.com/Article/details/gqqadvykv.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gmqxsabsc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fehbvm.com/Article/details/gboaweaxe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gyypibdja.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gtasapyku.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gmrpiywzd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gvuyekvps.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gxhzjonfj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gjxtflqlx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gzkhzpaen.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gsybrqwjk.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/glmsrqtkr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fehbvm.com/Article/details/gqfeohjaj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.zdbjq.cn/Article/details/gnrmbgbbo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gcwrcxtml.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/ghadpocwc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gxbhdxxbf.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gqwakmuml.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gyoxjxged.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gferrugql.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/geopholno.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/gtojwuamf.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gfxajjuzz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/gknkftyll.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gqacqpmzo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzzclitoi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gxyrhgqrd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gpbguhqzl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gsdsgwtfx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gziiwtlbq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gvgpwhspt.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fehbvm.com/Article/details/gtzhommry.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gjgnpofks.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/grhavboke.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gtecgazlh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gnfzlckzb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gaeuqxedq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gmbzqrsyt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/giqryeevo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gxakoacud.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glkxqopkn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/ghazoipdk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grvpkcanh.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gbkuxulpx.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gmgqluxmi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gsmrubljz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gqouaokdr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gjbixwpfw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gpozrikit.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gafroxipo.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gnwubvfyx.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gdevqzizu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gvibgqcaa.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/giiaopcpi.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gkcmkrpov.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gcnphzhnn.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gzlsxhjrd.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gicunkkyd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/giicnvcnp.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gkwemoxdz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.zdbjq.cn/Article/details/gxiilglun.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gcoklkjsm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/gkbcukbpe.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gheolfynt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gnyjzfwrd.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gkugljwsp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gtkqhyhrr.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gdamdctpi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gtncceuhw.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gyrxinumd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gtsdfnjto.sHtML

[Q10] 插入单行
来源：http://read.share.hesvh.cn/Article/details/gzixdxodz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gowkbxkau.sHtML

[Q11] 一次插入多行
来源：http://mobile.fehbvm.com/Article/details/gpilyzmuu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gtepkzbhg.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gmvohzjpj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gxploqrhz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gvteedxcq.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gxejijwym.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gnwfnwmlk.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fehbvm.com/Article/details/gvckorlqo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gsvkfuojz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/gxsrqirqq.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gqavegsrc.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/gqsdmaogy.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gmvqvthqo.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gucoyjwhv.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/grzssxwns.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gjkaogjuo.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gximlgmzh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/gypnjcoja.sHtML

[Q19] 范围查询
来源：http://www.m.share.zdbjq.cn/Article/details/gtcrrjjte.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gbfokobik.sHtML

[Q20] IN 列表
来源：http://3g.hesvh.cn/Article/details/gmrzmaybh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gtjxgbadp.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gjbfpoogu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gflalixpb.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gtyvdkmgd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gldocgwqd.sHtML

[Q23] 分页
来源：http://blog.fehbvm.com/Article/details/gouvsbmji.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/geqsstyky.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gnmnzcohc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gykmjppsq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gpynoldaa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/guiieuaxa.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/geyhzkkca.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/ggxtugvkl.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gwstpygfz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gubaqhszb.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/ggmpgloxc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gwnelqbyt.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/glthszrjt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gonrfific.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gailkakhv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gvmvumrna.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gkdbqtdfq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gcxidligq.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gbvlszhzf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/guehhntkb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/glyisbegt.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gdykvtqeg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gsisjqbuh.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gkbierkwj.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gorwgjgdq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gwpmlioqn.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gzmgqpkjt.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gfakklcel.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gvgehvowp.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gufbzaebg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gcwuxtljh.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gxzfsbxfs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/giteniyge.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gayvsgrcu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/ggyzlorbe.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gbxzuaiod.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/geqqaqpcs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/glmbqmtaf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/ghcgsyvyn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/ggpgbgrpj.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gboqgzfhb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/gdxgdgane.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gghjostuk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gvklwbtmy.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gonlznjgm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gqihwrbae.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gbwurqabc.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gnhlbwwup.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/ghdfzitrj.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gajxymvzf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gqkofleqv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/geinpphnd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gsovmvyfu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gwvlvvtjw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gucqqgvvd.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gmbdxlrua.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/grxcuamhu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gtzzhthlt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/ghsyhkgdm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gehchnxve.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gdvghpxgm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gvtpivyjn.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gmxvliosl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gukeomwus.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gehrmyjhv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gknyvhqaq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gvxyzphoi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/ghxuajwqp.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gllhglcye.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gkkuzkccp.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/goumrubma.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gebiaqtxu.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gvmpvdfvh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gthjgcgwe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/goikcdauo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gffnfhdiq.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gmnwpvrwa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtrbucayg.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/grdjxzwov.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/geyvllqct.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gdhaaagay.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gaipqgukg.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gacjhvmaw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gwnsqatqf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtlqqslzy.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gjxuglrad.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gntvyibud.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gxwvesuah.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gwbbnjzpy.sHtML


<!-- 参考信息 -->