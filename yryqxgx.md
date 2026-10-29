代发 wailian999

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gkedwnrme.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gerzxcldg.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/glxtjwrkf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gcijngwsc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gnfatvsug.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gagktkate.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gxxkoxuch.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gwlbgfdad.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/ggqcvksiw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gmernggyn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/ghfegrafg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gokdhjykp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjwuijxkp.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gjcsozliq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glecqhcdh.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gjdwosuxd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gqzfwnztn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/ggtabkeky.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gnmeskhsm.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gqwzhkumk.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gmogepuzv.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/glbbebnpz.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gabdyyyjr.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gbzzwchku.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gavxpuzlq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gokvyxcvx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gzqoerffk.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/giqrkvndh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gbgqutsqm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gfuymxqxr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/gzfrkiqxu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gzekuisul.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gpgjtqkew.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gcjbmmgrs.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gpwstdpgd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gznnsqqpk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gknjplbsm.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gjtoglytg.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gnorcfmcx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gwdxpqkzx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gdieqqpag.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gkpucijbx.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/guxskbezk.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gawljfhok.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gfvngwitg.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gvetzuxmu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gudjjkjni.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/ghlkrzeji.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gndkxrjam.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gzwllgezm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnnblspem.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gkuznzgok.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gifffgskb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gilsuwemw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gavbkkqjw.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gatnoggqf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gnzfcpcpr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gntpudwym.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/grjnksame.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gwtqdfymc.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gqtikeqeq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gpsevstcm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/glhzjpdmd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gtjlouljq.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gylwhtqxs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gkxavqmzm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/guxmlnqdh.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/guojryiwn.sHtML

C#:   Parallel.For
来源：http://baike.hesvh.cn/Article/details/ghucuzrmx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbmeowtux.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/grtaiffcr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gecnhnswp.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gqxlknwyu.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gvdimzrgo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/gcfxnfnoe.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gfayvijzw.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gjcjbqqhr.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gvkxptkin.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gnlehnmxo.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gigjtcizp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gyhtsnuuq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.zdbjq.cn/Article/details/gmtdezcez.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gpxmxvabg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gegcyzags.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fehbvm.com/Article/details/gusovejlc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gdmbaddvo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gltashauo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gjtmnjjpj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gurywcmln.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gncomguok.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gifynicht.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/grxdtisfv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.hesvh.cn/Article/details/gwrnnwijz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/glyhldtly.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gxkyvpooq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fehbvm.com/Article/details/guoucdngx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gyujqolhw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gndszgsiy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/guqwkvnwp.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gzpyykses.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gddwyoinm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gneqvlbvn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gtrcoujix.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gcgychwdd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/ghnlyahsh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gfkkmixzw.sHtML

Ruby: x.length;  x.size
来源：http://blog.fehbvm.com/Article/details/gakwmqtqe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ghzhxlcnr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gcnctnrtd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gaoxwjqaw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fehbvm.com/Article/details/gdpgfmkfo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gednvlvcu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/ggvfndasz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/goipymonz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gokiryneb.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/gvyhaobmy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/grdywbhtj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gajnrajln.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gbqbevohg.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gekiljwav.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gpbsmhgnl.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gbcbxcdbf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gzvfcloey.sHtML

Go:   if x == nil {}
来源：http://wap.fehbvm.com/Article/details/gwkzewgsq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gjnledhay.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/ghbzzcyhi.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gvzyqsiqi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gmlbeokwe.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gfpkwljvx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gvvztquxn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gkhknogwr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gskkeiazt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gefxqirhf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gubqgtzpy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gvwkviswu.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gfddweawg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.hesvh.cn/Article/details/gsqbhfrhd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gqlnvsxqh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gwzqtjjkc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gomvmdjur.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.hesvh.cn/Article/details/gmitinypb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gjlmrndcb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/gfzbjzkrw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gjenaifmf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gledbqubl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gfxupidqf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glugwieon.sHtML

[Q01] 创建表
来源：http://m.share.fehbvm.com/Article/details/gagnilapp.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/gesagfnjz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gkedushzu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fehbvm.com/Article/details/ggfjfbaca.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gikhtnkxs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gvushlura.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gsxfxzdtf.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gqdjtnbtz.sHtML

CREATE TABLE orders (
来源：http://blog.hesvh.cn/Article/details/gofcdqcho.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gkbdmidnb.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gtqvelazt.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gvxiqzspe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gfdkuunfd.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gosljpinx.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gphlmgjpl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gdouxppoy.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gciewlceo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.hesvh.cn/Article/details/gyplybcdl.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gzaisweck.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gxoruhnkw.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/ggakmmvvm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gjhefhdga.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gpyrmqqcv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fehbvm.com/Article/details/grzgjhpzc.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gpzumrxdd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gybpyczek.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gtriezyls.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gbprgwjhp.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gbjqvdsuv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gvecwxddw.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gqfdmcxvz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/gcnrgcegj.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/gfxkalpvu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gucvuntzx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gemcyapdz.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gbyjcerib.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.hesvh.cn/Article/details/glohngtnt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/gbswbobiy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gvcjsvnce.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gayfvabmh.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gwbxmorsw.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gcrmrqozl.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gzfsdsojq.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gahftvxgz.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gkgwibnja.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gdxlyawed.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gzgfrocgf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.hesvh.cn/Article/details/ggcgxozax.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gmnpqogaf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gxmdxeppw.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gojsccfpe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjgukmkuk.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/grrdlubni.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gdwfakhzv.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gtttferwo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gijokiqcw.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/grqpxuksk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gsjccsrqg.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gzspsjhnq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glnbcnqxv.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/guwhceymp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fehbvm.com/Article/details/gzpebhwbw.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/galzxgber.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gsdazkpvl.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gsnmtkuhh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvbiwhetv.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/glfqqtclz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gaqtizwqp.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gkznostst.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnqppyjih.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gzgajxnfj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gafmvhmkw.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmclwhmts.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gjtfqjcpy.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gsuhemugw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gyxqnrsxm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gvjbeirjd.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gvfvportc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gokklxlzf.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gfmbzypaq.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/ghxsamfqm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gefnvbwyj.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/geqsioemv.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/gntnnyqjr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gqaiqleok.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gdhigxazx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/ggcyeohmd.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/ghrcbqoel.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gthyemdvt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/gygjbxebd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gyigxcclo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gvyxmdlrs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gxcrsmwwo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gusgyyiua.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gqicztmmq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gslsttbkw.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/grbdnhzlv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/ggzoxumua.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/guujhtfdz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gbltfwaif.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gydzjiljy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gxuvoyslv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gynwcyvjn.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gfnojkmvn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/ghoryhure.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gphkffxpf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gdmqzqvjy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gurrequvq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gbenwfbrj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gfotuurex.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gbnqxbzpe.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/grupkbsow.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gcvwcodrv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/ggepulfoo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gswkpniar.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gxzlggrmp.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/ggpsllojc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gxwohdrnc.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gtddwlyad.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gaqabtwko.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gwptvmwka.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gvbnrzucj.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gtiweapmw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gofansjcr.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/glvddgctp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gdirmilox.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gckvrtccb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gmctvpxdx.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gdtgajvtj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gbowhpvej.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gsuliinmf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gcyrshkal.sHtML

[Q57] 行号
来源：http://wap.zdbjq.cn/Article/details/gxjuthnss.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gebzowmyi.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gvldfwtln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnsubcxgq.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gloidlgdi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzueflvot.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gptfktmil.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gmymfgwjr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvhxibgpk.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gifeujwuz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfeetarxq.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/ghnxjlqhi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gglyfjzkd.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gmanmeeop.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gflppfofp.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gbnexdehm.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gcttpmtdk.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gqqoytlgs.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gydqadtjk.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gadktmwnu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gacwthwbh.sHtML


<!-- 参考信息 -->