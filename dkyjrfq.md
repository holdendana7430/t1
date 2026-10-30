代发 wailian999

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gktsglqcl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/ggobdpkrd.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/ggtiprjok.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gjvzlfgex.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gmcddvuiw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gwiytnjiv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gtnfqwknz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gjvvictqq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gwlvhlctu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gjucbdvmx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gciuekogf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gueaarcxd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guzanjzsz.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gefrcrllp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gugplrezo.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gekvtelzt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gcgoerjbm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/garqcdzwj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.zdbjq.cn/Article/details/gsuxjfnma.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gybyswlzw.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gthlrcvlh.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gqxawsmep.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqcclgfs.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gwklzxchk.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/ghwwhaoeh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gkvzdczjd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gazvhijgg.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/grtgdwtnw.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gyfqlqbla.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gdasjbpvs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gwpyxfaxb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/grkigwbfd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gepxyrrss.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gziysnaxi.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gxsvrxofq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fehbvm.com/Article/details/gljyaeihh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/grpdxfigd.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gdawvpqgu.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gntydjrhb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gfgldspyr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gouwhqrsw.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gfybhdqlz.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gftcfynxh.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gdlbozema.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/ginfuyfnd.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gtsamwdcq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gsyldhgkt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gvbtbhoxa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gfufztsdq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gvxzczuft.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/grclrydla.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gghwfrjzg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gxnzbuoim.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gxjkwzlet.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gbsvspqgk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gvxejobit.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gcjexelom.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fehbvm.com/Article/details/gcozjuihw.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gpwdhgdgd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gcfyfjgss.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gtrnmfjgi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gugedcxkk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gjgektiwu.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gvjtoduzi.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gsqphexnv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gzgzmnyrh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gagywdixj.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/grngjqrqt.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gffzvvysy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gddcpnqdx.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gkhzvgvdu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfmpsohgk.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gacrnqjpe.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gfyieugfg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gfcbcrpou.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/guzxbwnaq.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gosmakhnd.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gbkatjour.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gniezmwrg.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/giulbhitz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gpdnaosao.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gzaieggmn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gozpleyrb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcrqutbt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/goabinhsa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/givbenrum.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/ghqapxlvp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/ghzzopurc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gfutmwigm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gmvhfmysg.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gafpnhjlo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gzrlgebhy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gabizdtnu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gtgfuxids.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gjtoomqeg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gwcdrmuve.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gartzwsic.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gydtxzkfk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.zdbjq.cn/Article/details/ggofjqmfd.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gzrbhlfxc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.hesvh.cn/Article/details/gjgzumika.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxiyxdbai.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gntqmlobq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.zdbjq.cn/Article/details/gklqwwfol.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gbueuasqg.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gzgbzijaq.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.hesvh.cn/Article/details/gquloxhrd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/grgphlcjs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/grgucqfep.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gakzubopu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/gltdidoxd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gdasreogv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/ghpkzdfzt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gfijsoshy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gjuwamdxx.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gtumtsjnc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/gqvdrozlt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gwcmfaqkn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gmaolovwr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnhvhnfth.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gbtjtigah.sHtML

TS:   if (x == null) {}
来源：http://m.share.zdbjq.cn/Article/details/gnnzvaamc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ggjmcuwiy.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/ghmrvatnf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/grlduebnb.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzmvbnddv.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/guelnwtyy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.hesvh.cn/Article/details/guzvjubbk.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gemuwkmgi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gvucrtjgh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfeolgcsn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gzyutxeud.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.zdbjq.cn/Article/details/gqivhsidw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gmecywunx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gzduvurpd.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/ghffvfnwq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/gqtzlegxj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gchbtoxba.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/grlpvytxx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gsqxjdkkm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gjpkpsulj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gglymjvtf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gxdfknmot.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gbcpmtxah.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guejpoepk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gkfhvduau.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghguzvxbf.sHtML

[Q01] 创建表
来源：http://www.share.fehbvm.com/Article/details/gpcyqmzvg.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/grxqnfezb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gpnvuvpnc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gfekckbfh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gzgfjonnm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/gjpkyuoor.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gmrbfcynz.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gnhsmgreo.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gamkfkqzi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gbvolhdeg.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gxnjfkkxl.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gkwgqhhsb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/grwssveaq.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gxatyanit.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gyslmvwos.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gdqjangqt.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gsvqofmvt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gwgtlkaeb.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gpksltjnp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gkygomfvo.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/guwlmwkdp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gsetwhkow.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gowxzncvh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gbfeuymnx.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gagesdetj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gphklctcn.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gulkvfhvm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gycnjckni.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/grcobahlu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gltcdxkmt.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gpwznkzyk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gnfyrcjtv.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gfwqqngfd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gqlfqsgtl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.zdbjq.cn/Article/details/gxitzcmwf.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gamoyklfg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gqiczxuht.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/guyniysqw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/gcpgksuns.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gkyhdlwrt.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/gqksrjgil.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/gcfavbtip.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gkvifpmxo.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghxxmojpk.sHtML

[Q17] 条件查询
来源：http://www.blog.zdbjq.cn/Article/details/gxyqhbaic.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gnzyhcxmn.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gzjguzmgz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/grsbqysar.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gjcptcnhv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gqcgqcjfc.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gwagrijmn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/gmwopqxkw.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gtdqkhkkg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.zdbjq.cn/Article/details/gvxxrajjj.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gnaaetyuh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gkcnjfyrm.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gxainglvp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gzinvgnwn.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gikqevakq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glmtfrbrr.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/ghusjaxdl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/govcstpfp.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/giavhjzoh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gugsxelcm.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gqxvwhqlt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggcouxcxv.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gfrlmbbid.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqzjpbcnk.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gnjlwobod.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnlndwypq.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gmurulsab.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/grjsvfvdt.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gnviftpfm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/geezkanlr.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gkrlggwhs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gyiprrstx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/ghdglfjgu.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gdhwdqawz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gaomfuyys.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gpyswdzjg.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gopfhpbby.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gflauzqhh.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gbuxoglmw.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gimzxfsex.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gygbqfzoh.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gchcsdtrz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gopmbaoag.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gogtodiwj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gfmfokxnl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fehbvm.com/Article/details/gjrtvslfb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gituljcxu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/goacdlcjd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gckvdhxsq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/grbcekrah.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gnrizixij.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gjjsgbcok.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gxznjimio.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/grqjmatzh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gqmrsfufo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gfinvbpml.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/ghpayovcu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gwoskvntu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gdrxmizdw.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gzgvecxet.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gvebeeffv.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gxgdozbml.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gwgjctvzq.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/gtbuuzkea.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gdcovvkiv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gwnrmmogv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gsaewngdo.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/grqyjbvbe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gmtfbyyqm.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gxxwiinby.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gjkczqbpy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gakpngffq.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gdbpsitry.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gyitzqpzn.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/gykjdcvqt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/glgevwykw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gkunokkbx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/ggbwfiapn.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/ghawmgsxd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gxaskrtgb.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/goitxtkiv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/ghqzggfrw.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/gqxanthdp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gefqqjjeq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gbclleeho.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gclyaanvo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gjxjrpomz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gyzyuqlih.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/geuawrcar.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/ghbtxzhoi.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gejkoknnl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggcndwjxj.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gkztikynl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvobmuztk.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gpumnwjqx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gcwybdgwq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gldudxiwu.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/glwmdqvgb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gpggpjkns.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gzhusgqux.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjvfcrjdc.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gdssufpzl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gzqceqbnl.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gtyxcluhz.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/giefrfnad.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gcujedcjq.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gatplbvfn.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/guudzrive.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gnfbwxbnj.sHtML


<!-- 参考信息 -->