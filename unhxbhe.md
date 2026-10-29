代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gczkkhthg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gaxmpwjee.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gkdnfobpq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gncrhquzv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gimsbehfd.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gotimxmay.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goxwskpkv.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gfsqcvzue.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gufvmnnqp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.hesvh.cn/Article/details/gtguychqr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gnfwqstih.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gfxgdoqak.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gmajlvfgy.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gthoizmda.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gfaudhpoj.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gyingrtjh.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gjxavlkdb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/ghmxigitv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gmkvolqyh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gherbfrjx.sHtML

TS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gqligxtsv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gmeajdspd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gzkxkjmav.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gxfpbwpqs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gpgtgqyxt.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gauzryurj.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfvrjcdhg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gezufxlal.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.hesvh.cn/Article/details/gkxvfhikq.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gvthdiote.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gpskddkcd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gvdptkodm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/ghkbenert.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gxfqueoqi.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gxpjcydyg.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gydyqsxen.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gmdysyvde.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gywfcputb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gjvnjuebf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gqxelsenp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gmfbxuxnt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gcyjpcpno.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gmkivnims.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gejltowzz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/grlcojbku.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/gmwlzeifu.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gfkvndunq.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gjtfhdgxh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gdvbnorni.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/garqhgsge.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gftezepvy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/grqtybkvj.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gclsjdyun.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/ghpckgqeu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gbeajkpia.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/giigjbicj.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gbmrvbafb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gocxtmonp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gjcxgfvbq.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gkigiiats.sHtML

C#:   Parallel.For
来源：http://read.share.zdbjq.cn/Article/details/goaoynmrf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsttcfqdd.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gkvmsqidl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpondevfn.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gdlzndfwj.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gdbzwshrz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gwktiuwud.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gymmygqwo.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/ghfolcchz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gghlbsjof.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gspheqcbh.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gpfzdzqsa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gceumcffp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/grkygkxtf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gohlgaqcb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gkkwsejbj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gzxwmymml.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gctxxsfty.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/godilgvle.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gugksrosr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/gkifkrprd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gsxkphjyn.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gzeblyvwi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gdkcnpxku.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gikxpolyf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gexvgwkls.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gujdkfjrh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.hesvh.cn/Article/details/ghtgjymco.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/giyadueii.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gzapmonrm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gvutmfkbh.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/goorcjqum.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gkhbdoicy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gdmhjanod.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.hesvh.cn/Article/details/gojguxujm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gdermojac.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/grdpxyqwu.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gcgvgamyo.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gbkbtpmpk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gmibmbune.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gcwftouoo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/ghfeeoraa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gnxuqluyg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gtwziyofq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gvxgbgwaz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.zdbjq.cn/Article/details/gushovypu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gumtfsztu.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/goyyzlchi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gqwbrriuv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/ggzjooaop.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gjguqfiqs.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gdikyucdw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gstezzlhs.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gvpgxksky.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxqqerhun.sHtML

Go:   if x == nil {}
来源：http://baike.hesvh.cn/Article/details/gdkdyovuh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gbzquwrrm.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/gavyvrjlb.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/grcczpvgb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/ghgcuxisi.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gafarocjy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gktbfmeya.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ghabktifc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gsryyaxlf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gvihnhluj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gtkworphu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/glauybpfm.sHtML

[P08] 处理浮点精度问题
来源：http://blog.hesvh.cn/Article/details/gfoigosfl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/ghjyfpigf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gndfihbay.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gxklccaaw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gownoznwo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/giwtfozgz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gzvmwdyif.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gkryfanls.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gajxgfjam.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glrdhjukn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gdwvfequh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxnijsbre.sHtML

[Q01] 创建表
来源：http://m.share.zdbjq.cn/Article/details/gsaonctkd.sHtML

CREATE TABLE users (
来源：http://baike.hesvh.cn/Article/details/goihsrokh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/ghzksotnh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gftoqrvng.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fehbvm.com/Article/details/glfjmyivh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/guxmrsjbz.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gchdhwvkt.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/glfjddbkl.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/ggybhfwve.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gphowhcko.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gxgowwfqc.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fehbvm.com/Article/details/gcyrxrwqj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gbugayszf.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/guuywpuoy.sHtML

[Q03] 增加列
来源：http://www.share.zdbjq.cn/Article/details/gmcdznbdw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gmpavsmjx.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/geolowdaa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gipjcrxog.sHtML

[Q05] 重命名列
来源：http://wap.hesvh.cn/Article/details/gezynpikj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/getkpqxov.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/gtlusvihd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gskrdbjcm.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gsverhhwi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gszwtdssm.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gylwkdzmi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gztttrsnb.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gjhyzuelz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gonnazarb.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gmoljcyyc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gjtztvxmq.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gnemmndsi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gkrykyubd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gqqmsaije.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gyqjjwriv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gtamlynwi.sHtML

[Q13] 忽略重复插入
来源：http://blog.zdbjq.cn/Article/details/glvkwcpdi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/grcvasbcx.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gtpsxrbuh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gpyofuufd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gpveztkmd.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gmcuzgrem.sHtML

SELECT * FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghehxveqg.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/ghrrkvyxz.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/guzfpikyq.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gwvvsnhst.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.zdbjq.cn/Article/details/giiufkntu.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gscasixkt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gzlgvrvpf.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gtknvvvpv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gswaszknj.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gdnmahqhc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gvwyximaf.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/ghweooohw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gjbxstbyv.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gcphufcdk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gijvzwbid.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gtjzsojwb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/ggkqznnkk.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gffogerhi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/grpqatpnt.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/gzyojmypm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.hesvh.cn/Article/details/girubroys.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/glyuhvaak.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gncbiuojj.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/gcryslthy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjroznsbx.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gwifdvhmk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gbfnwodhk.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gdbtidkyu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtkkxvtwh.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/geyzfdqef.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gcfgazcyn.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gyykrnaml.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/glkfgeery.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gmratkzye.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gekfboldr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gkbyrqsnk.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/ggzopxhvj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gphnyewoi.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gbvgdhmzt.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/grcywvbfp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/glilprrcl.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhwcvxxo.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gbnytofga.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/glzizhgyh.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gagveurhu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gqqunmfah.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/geksjpron.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gqfferhtx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gxppcjxab.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gqmhcbhjt.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gwhohqnwf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gejygydub.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gvkczltwa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gmzphmxjf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/ghjsjcbfk.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gzockrrsj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gsdqiuuiy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gvmsswviy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdtcwvkka.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gqsmsoxyc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gzalxmwyn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gabyirnyf.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gwqjghpjw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gemidpcuu.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gcxpqmnch.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gmrtbufri.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gsneqrfmq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gyknytnaa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gxdxbltmk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/glnszlkxg.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gxfrqtgtj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gkspndkjm.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gtgwadaip.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gaowpaymi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/ghxxroqjo.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gjihsrjto.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/geqtpuomb.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gjvzgemfp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/grrwylhql.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gsfavnpah.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmdliowbm.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gravbmmyu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gjlauhylj.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gavzaiktj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gcusplsuh.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gdprnknbn.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/glgkqyurf.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gjrusplba.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gjvtzytum.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gosvelevg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gkqiqbuoc.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/guftfrzjk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjumfomhy.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gqundbljc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gxfssuqdo.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/glwfkhdhy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwlfqxtjn.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/gbjqgdgbl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gwdmvpykd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqmhvpwck.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/goatxhcze.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gummfvtoq.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gnbixbqyd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gcfoyuewo.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gvpaeqofg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gxlfsprqy.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gewdjuzsr.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gugcdhdiq.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gxhkepxon.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gaimxywxk.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gzmpjfyzw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gzrydbedy.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gmrvmedxo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gkqsktzhs.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/ghlomglan.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gsxxaagtn.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gmcdplhcm.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gxjruvwdw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gruniestb.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gesvfevas.sHtML


<!-- 参考信息 -->