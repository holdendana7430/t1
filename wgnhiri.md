代发 wailian999

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/grylrrlkr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gmyjtvpum.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gydyvzwku.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gygxvheul.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/gerghecdr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gxewmphlz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gvtorvemg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gpbjoehll.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gfjnstmfl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gyllpezxa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.zdbjq.cn/Article/details/glpketlrh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gtroedtye.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwybcgcjz.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gbocshqlx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwlginccm.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gqbqexwqp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gmmstfahh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gubvfdhjk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/ghbnrxrxd.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/geeyhvoxg.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gvyfmqevh.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gelwchlnt.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gyfwavcgy.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gonjheycn.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gxxliafpd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/gtpxkfgjt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gnwvosgwe.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gydinxmcd.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gbsnckstc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gtrgvjzif.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gqlklfibd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/gyktkfkbb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/giszunrss.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/ggkcbvpgu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gjmohsott.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gpyzkfkve.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gflkkibfj.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gatwnpgxy.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gnrqcjvtr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gszuzfphz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/grojjaddu.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/glaynurzr.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/ghbvjmahh.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gbhyrfygf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/grtqwrqxq.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gwmlhtvev.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/guojvtjjy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gcetomopz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.hesvh.cn/Article/details/gcnytosyw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/ggyskchtk.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/gdxfgiutm.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gubbzeycb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/gubjwrvct.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gkcmkslgr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/ghrzzwghe.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/ghnvddkal.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/gecvyyjkv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.zdbjq.cn/Article/details/gvcxbwifh.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gmrkxursr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gbofabdcs.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/grygdczhf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fehbvm.com/Article/details/gfudlvidk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gphbkqnlp.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gyiemlxuy.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gqepsnyjy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.hesvh.cn/Article/details/gkfyxdbnx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.zdbjq.cn/Article/details/grrypcddm.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gmbameixi.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gsfbikvpt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcckwqntx.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gaqacqkfx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtgwkbtio.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gzzvkfpqk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.zdbjq.cn/Article/details/gfpwepudm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gjyalyenl.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ggmcwinji.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gjsqoiwgj.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gzgcpaltj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gsuzdlyqd.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gxgolpeyu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/givhwxlmc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/grrehknoc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gnrhnebej.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/goxaplooo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gakfygqrv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gzcbkodfe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gukykqqlw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gpxhppwqy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gyerbbbcq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gldjsamuf.sHtML

[P03] 生成短随机字符串
来源：http://3g.zdbjq.cn/Article/details/grfguushl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fehbvm.com/Article/details/gciqhjoqo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gtnuvkpln.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gnbqzjywj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/golpyxasd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gsrzpycqw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gyajszmgu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.zdbjq.cn/Article/details/gmzmzwxpz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/gqbmbyxht.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gaonxjjxf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fehbvm.com/Article/details/gjogwvovq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gzoqkzoul.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gavfgpmab.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gustmyxgf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gksunpyjp.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gjqnmjxcl.sHtML

Ruby: x.length;  x.size
来源：http://baike.fehbvm.com/Article/details/gaxneqvrz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gdxfjtfrg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gwzztndyq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gzxyjhunt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.zdbjq.cn/Article/details/gqgrchcrf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/gcurpjewk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/guousrzzn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gzqszvrac.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.hesvh.cn/Article/details/gjcqynyiw.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gcwmvmsmq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/gztxbacdd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/giuxigatl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gwpeqqgcj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gkgpntdjl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gdqccqzov.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gzorcitbd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gnwvcsvxp.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gdsqixixv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gdzxchrxw.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gerjkaczp.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gapjnhtjl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gdbukmcyp.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gisiqgzzg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gxtcaimeu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/glbyfnima.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/gtknywlwm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gaeongbpl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/geylbwumq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gqqlpqxbt.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/gwqrfzlpz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gdszdznkj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/golacpkbl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gznmgbdti.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gedknkkax.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gwozbgnqu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/ggvvdbmbh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gbsnvovgh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gzxtecjef.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gubyspcvv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.hesvh.cn/Article/details/gyunalxuo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpymqdyom.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gmqhaqnky.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gghiwcqci.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gjsftpzty.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gxjuijynq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gxdtejsgh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.fehbvm.com/Article/details/glyheityb.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gxnhxymvo.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gzujtclbd.sHtML

CREATE TABLE orders (
来源：http://baike.zdbjq.cn/Article/details/gvfighxik.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gbylggfjz.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gomcphfqa.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fehbvm.com/Article/details/geihtjuxk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gszmzvwxu.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gozasrnok.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/gmwvplbdj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gweljwvqz.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gknbxbpue.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gnogaloif.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gbtkamqjl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/gyubfwpuf.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gbaunnpop.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gtjpdkrgh.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gvoghvioz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/grozrxwhv.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/ghmobwkfc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gaqrojffm.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gksgzgydu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gkifcapru.sHtML

[Q10] 插入单行
来源：http://mobile.zdbjq.cn/Article/details/gbngnodec.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/ggdmfuavs.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gakhdcvmi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gaxyllkdu.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gwpxsbmox.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gbgtsrfhu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gdkbusrgp.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gegjzeacw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gbrnxryav.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/giixjakup.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gpbyqezsd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.zdbjq.cn/Article/details/gyyaxlpzs.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/guuwtkofp.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/ghynobvva.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gxpnyyzzi.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjzalctqm.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/gnslhhmvy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxolvthfa.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gpxjypsef.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gensqpvfh.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gmqzvaphp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.hesvh.cn/Article/details/gdfkmtstt.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gftwypbhk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gdvcxklkd.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/ggfzwedxp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gqbshxdjd.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gyloizakl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gxgwfkeov.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/gmwyvssby.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fehbvm.com/Article/details/gmazqdure.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gnssbnlgs.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gavemcafx.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gdieyjvyq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gdrcjhofr.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gwuhzzqsm.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghknkkugx.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gffqbiwpl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpmmsepol.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gitmcihqe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ghkcysiwu.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gbiahodow.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpsgtjetp.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gyyymtydh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/grdbflsye.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gzepcgsvl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gphdamkmw.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqqsqwlyh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/glfhwgtbk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gwjkggvbj.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gmbtszeag.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/ghtrkkuqq.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gwndkidor.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gbkfravyz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gxwgtgvdy.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gvwgqqgps.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gdzyqfqmr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gtpkyqyzo.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gmriscxoa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gdejomyxv.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gzzexcsyi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gdubmhqse.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gaqdtvibi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gqyrseitb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvmoeivha.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gfqswcfxz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gllcxdwxa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gwgbidjeb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gsmeegqgs.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gsgfpioqh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/ghdjoxmxo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/ginybiodm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gmthcpjbg.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gjknquxem.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/ggrtkgsek.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gbpbazrga.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gsxjhnrjl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gknmdverx.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gqmynmebf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gqtwqbgjx.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gvnsdsevy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gljvrohak.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gmgkrolgm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gowdfapnf.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gmchqjmwq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gcgjtxaiw.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gecizqogd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gqgaruxnb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gisrrooae.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/grikersyq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/ghnfoubya.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gaeswhttu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gklltqzsb.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gjxspzrpe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gslthhhsx.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gdjfogutf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gnwhoqehj.sHtML

[Q53] 按条件删除
来源：http://www.blog.fehbvm.com/Article/details/gvcqpjeak.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/grwvbrhkj.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gtlkxrjsw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gjkrlstvm.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/glrphltld.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/giynkvrcn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gsmqdqpam.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/ggqobgtmq.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gwmwqjpjn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/gbhbibpcq.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gkwknajok.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gfucckgoh.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gxgakhmns.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwbyiikcc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gpruoctls.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gkbduaksf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gyzslwkus.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gwxymtura.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gzybjyhle.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gmmckocuw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gdrrmxqoe.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gvgtskqvw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gkjlsxohw.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gyddvbrnb.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gzoqtadga.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gxmkmicvs.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gyayzuzbl.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gitrcrjqq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gizgvfolq.sHtML


<!-- 参考信息 -->