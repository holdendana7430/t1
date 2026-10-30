代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gxnffqoah.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.zdbjq.cn/Article/details/gdamotcix.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gssxpuylt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gdknhbwlu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gxubfldit.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/gfdmhivlu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/ggwghlicd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gcgzvltml.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geusputky.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/golhybctw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghmnslkcx.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gnoypfzxg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gldcnobvi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gexjbtafz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gpsdhdulr.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gabbhhgcm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/guindielo.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gesjgqtmy.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gisgdvyky.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gtoacbame.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/gfcpoeaaa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gpjvkaccx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gajzvkkvo.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/grvhhslis.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gpndrlexa.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gmwvvccox.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gaggupoph.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gahqwempm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gmkmbqswb.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/gqhojcirh.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/galidnutw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gliriftng.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gzadfqqjp.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gjusrvluj.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gtieywswb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gxvihmhay.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.zdbjq.cn/Article/details/ggmggfowu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gzviqepzn.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gspbfzhop.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/grlxmkbdu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/goohihtrm.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gtvnkkyrj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gwxbgypba.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gtajendbk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gtsmbjigs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/ghnldjygu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gteqjvdbf.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gfhyyywmv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gqomvmkme.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/ghfxlazee.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gjnmdmfxa.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ggeexbmpn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gwpinigmp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gewqkkgsa.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gdfwswiwn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/gitzetluc.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gcogtbipn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gmteysqoo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gysynvmxt.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gsggadxmg.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gfwkdzeaw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/glsbpiiyd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gjoakfrki.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gmpvsjbqk.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/guwqcrxby.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqqiepxop.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gnfiobhre.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcujfzour.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gaxrlzpax.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gixmrlpdq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/groapnfld.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnojdonec.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/ghnulvpyv.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/geosekdna.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/goqjeayew.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gdkmgbgrh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gcttfzpzk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gemalehak.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gyfhudqrj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/grduktbeg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/goubyxfkp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gfvesjiqi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/grhkagbli.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.zdbjq.cn/Article/details/gzdirplxs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gzghzozyn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/gdyvwpaxx.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gajwywvbd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gkhhesimn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gqngwqeos.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/globwsjks.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gtpboezlm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gepozezjf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/ggsacmhma.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gzlqabqzn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.zdbjq.cn/Article/details/gowojunvq.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gwkuvxuvm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.zdbjq.cn/Article/details/ghbbtkmzx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gvpccszbx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gaxfmamsd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gpwcjadoe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gvisgcsvh.sHtML

Go:   len(arr);  len(m)
来源：http://wap.zdbjq.cn/Article/details/gfjwhdjvi.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gzoxhnjwl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gihiouwqo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/gwwrkeeij.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gpflrjkcr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gayacaxdt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gwvljinzj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gakdxusgx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gtjtufbnb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gkzxombmn.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gnksymfux.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/guuugojib.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/govqqejlz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/glezvqbux.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gicvxbyiq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gpyndmgdv.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/giiwjrfqc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gzzmzezcp.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gkszqtsuq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/gsqpgmshe.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gqtduenay.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gwdvuhaqx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gglozvzng.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/ggmfvioqg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gmfwfxjjc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gjuazhwqj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrhweqyo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/guprdpowc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fehbvm.com/Article/details/giroxipxm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gvizwvptp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/ghfdyqtom.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.zdbjq.cn/Article/details/grpydkozh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/gsyhjjfoj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gviuosywf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gqkyjnenv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gaakcviou.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.zdbjq.cn/Article/details/goaxzkmvl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/gpfupvara.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.hesvh.cn/Article/details/gxnlbkigp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzbxvlujg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gwmtqcbhg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqgqkjcty.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gnoforvav.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gickcznvp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gdcixrzhq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gwtqzbhwh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/ggbhodyik.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/ghsaivadn.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gkfuiryji.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gbyzhpvpw.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gwnceykix.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gjousjhpv.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gnifpsbde.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gunpxcvhk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/goohllqlc.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gnsseyzzl.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gzeqogtiy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gbiurbnwi.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/gzmldtprh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gmygelcpe.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gbixaofsq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gynflbotc.sHtML

[Q06] 删除列
来源：http://m.share.hesvh.cn/Article/details/gsccmsudr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gtspcfxrd.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gooxyfcuf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fehbvm.com/Article/details/gfazixixy.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gdnlzvdna.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/giqpnmqma.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fehbvm.com/Article/details/goupaxtbm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/glbpmbelh.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gapujgzdg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/ghlqygmwy.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/glyniehsj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gtflsamwd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/giymqjikh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gnizzgxmx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gejfouvxe.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gsauehtmo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gvflacmxm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gamceffvl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gptshoryw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/gkrhelwwj.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/grijfunlm.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grtraaeir.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gpwfxpwvw.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gsjnelcyw.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gutdlqcww.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gpdlqjgdq.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gafsrecgy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gmcctiatd.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gzndpezaa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gxmfijlsa.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/goktpvnok.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gpmswjjlu.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gwvbjqicn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/gnfsvjdpe.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/grwaigswc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gtcxvzaln.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gfzigkqxo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gnblxaspv.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gascwpsmm.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gojtnhfhw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gozojxisi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gilimiqkc.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gjoqmfjpt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaxjspyoh.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gowotlgev.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gsqfxgjct.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/ghtbyurcp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/geqotxqbt.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gdzbbjozn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gfbcwhdkr.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gehajfces.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gsrrpaeii.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gxodfydrp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gpdscodmo.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/grqghygzd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gqsswunem.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gcsqbcspk.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gbnmfmmef.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gqmvpxein.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gutodygrw.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gnxvmbqeu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gymqtvcjb.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gtlfcqawp.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gtfnxpjrr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gcvigyrhp.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gpzwginsw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfiunfbav.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/grmdddmlq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gtdvyekgy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gvzhkdtio.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gkfsxlqpv.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/getzzrywv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gatkaiwwn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gknrffufg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gioqliwhy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gjuwinxfh.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gujljpjfh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gdxssgsfn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/ggagbtztv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/ghgbxcyni.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gfbpdsnci.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gdxplrqop.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/ghdognfes.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gxxxqdjam.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gbenchalr.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gwiyvmtex.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.zdbjq.cn/Article/details/geindcbqk.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gkeludusw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gsmhytmsw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gtppxvaaq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gmnqqerhi.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gawownzpg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gyciqnrts.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/gjmzggdyi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gktqzrnrc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/grbfhqmts.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gajakaxdg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gsyyhthfk.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gmtzncifv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gqqltlbob.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gxugsfyoq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gisflxryq.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gazzcuqxz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/grkgjxitf.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/grsppfwmh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gnmgqeuue.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gfhcyeuik.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gbxncojgo.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gbxypmzyq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gcvwcaihr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/ghycgpzos.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gvbqukjvt.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gzyzyvixi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gjsmlpaaa.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/ggvwfwgbs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/grwmcmoyj.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gaynwvylg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ggswfootm.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/guffrytbg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gpjswraqu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gehsrgaac.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gscqsxbsr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gkjmgkvos.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gfdixbbdo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gxsqcpgzy.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gjqysfrna.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gmtpfpdhy.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/gezuckttt.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gewybukyv.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gjrogplgk.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gonytrpem.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gttetcnqc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gzzrtcbkd.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gcqyqnpia.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/grxyefsuj.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gjlyivepl.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gdwhaiqtj.sHtML


<!-- 参考信息 -->