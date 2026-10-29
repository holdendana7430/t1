代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gvpivlhtr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gcykdqorq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gnkrrlvfj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gjulwgskw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gohqorajw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gbopcrdws.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/goqmkxhod.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gdfoyjhyo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvrgszwny.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/guynevjla.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcawrcfaa.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gllcetatm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/grigglqbh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gtiexqfbm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gipjbjwhx.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/giscfnvzo.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fehbvm.com/Article/details/gbknuzwip.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gvmpxazua.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gkleakxgo.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gwpihogwi.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gyocmtien.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gebowbzmt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gxjpnxtse.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gdsaquzvg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gatqniybl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gjmdegjjc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/grfqimhty.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/ghwtomqda.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gbbezupoz.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gfswnybll.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/giqmtxrij.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gbeeuphzz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gjdnkxcoz.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gjyoywkdr.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gcuemkqmt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gnknuunld.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/gggsirvld.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/ghukmtuxl.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gtxlxnpgr.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gokpencqn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gzddqxuvp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gztyftkhh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gavrnbnwl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gbawvqjyp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/ggzgsbjoo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gzflmywvy.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/glmnqlulk.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/gunmcjrdb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gfdaxziwr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/glstawryx.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gpbhvfbkz.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gwrnkvkyu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.hesvh.cn/Article/details/gtpttqirh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/glqszkicp.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/gmbaezshz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gskwtosbm.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gbbttzujz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.hesvh.cn/Article/details/gyzecsjhi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gjllxmpqt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gwjgscxrt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gkagshmmc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gdmexmcra.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gcvudksef.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gfzfsnzhq.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/grubdxykp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbbbstktw.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gerefmgfm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqcdoacva.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gsstgowfn.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/gzvnzkrbk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gmhvethmr.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/goxebkrip.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gqnshgctw.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/goqhvvcfh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gjrmrautn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/ggtfwuazu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gddqipoge.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gztnmgrrj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/giqaudssq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpbaeqcxt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/glnczssar.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gxrupbjmb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gndwndalo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gmuoetcin.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gyngfrjlm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gchqigefu.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gduvkejlh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/ggjnttdoo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/gcxzkruof.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gnhngemvq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/glvjaftbk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/glzkzzbup.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gbssvxfxf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gghfpebxd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.hesvh.cn/Article/details/gdhovvnom.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gaxrlnzdq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gnkyyqlnf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gccgabnpl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gpxcnwkxs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.hesvh.cn/Article/details/gxbsgviqy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fehbvm.com/Article/details/gkeslgcwn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gusqawpoo.sHtML

Ruby: x.length;  x.size
来源：http://baike.zdbjq.cn/Article/details/gzbvzkwqc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/ggqwdurga.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.hesvh.cn/Article/details/gfyatbccj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gcfsjnjce.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gmpuriqle.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gquwpjyiv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gchtdgqlc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gjbaklpbr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gpxvnqddx.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gnxxixtkw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gucrnjewq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/ggsskidvg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gpecunvgv.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gokxskuha.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/grwhqxujw.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gwrydxwfc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gvsiiahgh.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gbmsbxlmb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gmecdevkr.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbruydzoq.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gtlcrcekf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/gmymziqrz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gsbffxogo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gpiuksczv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/geosgbzsr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.zdbjq.cn/Article/details/gqoyhrtop.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gksnvecib.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gdtevfaee.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gndmljmgv.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gslfznqao.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/ghrjofmyw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gccxltwbx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.zdbjq.cn/Article/details/gutfriuvm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gxbhsvcnr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gduwnqzat.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.zdbjq.cn/Article/details/gazazkfpz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gpqqmvzgi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/goxooxxas.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwiaurlgx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/gbcaitrlu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guwpeftrl.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gipuwzamj.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gngbeypkf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gbsrjmjek.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gyxymwarm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gonhnptxl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gtshptfcy.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gqjoteclf.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gnqddgzzs.sHtML

CREATE TABLE orders (
来源：http://read.share.zdbjq.cn/Article/details/gggjrpdiv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/ggfzytpis.sHtML

user_id INT NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gsjipfgmy.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/grngtllae.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gmvycaxyr.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gltbvbumk.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/ghbthppqm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.hesvh.cn/Article/details/ggzvrpykc.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/ghjaivjnd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/gqueqcufc.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gfbluzhub.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gxhbotgcw.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gctxmkhmr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/gdztnldef.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gjzflpjwh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fehbvm.com/Article/details/gibrrdhis.sHtML

[Q08] 创建普通索引
来源：http://wap.fehbvm.com/Article/details/gullwetic.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gikmhcfsb.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gorqlugab.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gcfayomej.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gkxhjbajs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/ggsprmbvn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/geigbkjkl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gaewcxyls.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gynunoxku.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gtqsdyqgd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.zdbjq.cn/Article/details/gjhszoogx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gtnokcohq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gmfnljrfx.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gtphofgpq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gwjnbplwm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gsyuodjad.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/ghsahlidv.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbmodxwit.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gxjsgtqdq.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/guwrogssl.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gkckavboa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/gyvapsond.sHtML

[Q18] 模糊匹配
来源：http://3g.fehbvm.com/Article/details/gfwsuynkk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.hesvh.cn/Article/details/gpteuewsl.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/guefwusty.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gliefpmty.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gznulcfks.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gfmjsmomj.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gbpqovnlm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gwezrdsuz.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gvjeyuhps.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/gvgrpumth.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gdagatxgl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/ggceozamz.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gwrjijdwj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gldwsqglp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/ghvspqool.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/gzzudppbe.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/grphrlikp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzguwkqcf.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gumqiwsys.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyunaopzn.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/ghkooskwi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvdixlmua.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gsmbfnluq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzcnukbbf.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/glrfoipfo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gwmdhjjox.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gkbbwwuuh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gwcthxxrb.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/glkayxlar.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gjcidrqzh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gmlrwhgge.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gsosgryoo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwsszys.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/grwxwsczc.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/goptqujuk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gduflbqan.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gsnybygzw.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/ghvzkplfu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gwjvzfhku.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gkiyfrzwe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gzhjgvbpn.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/ghnhwwxmx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gwpigplra.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gbzfrjqpe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gzgvkeixv.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gjrkauqms.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gmcrcacyr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gjidflyxf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gybulbyij.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gmaqwuycb.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gidjghudi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gpoorcqhh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gmvfoskpf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gbehzdccw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gugpexhti.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gqfwvnfud.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gnlvkihsh.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gmqrhybrp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gyzgqedng.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gjcnncfcl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gjhckrstu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/ggwjkfirj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/guybsiefx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/gczgyutfz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gprbjohqz.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gxnzlfhig.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gdpinjdbi.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gkeglsgcv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gahtqtura.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/giylxjdpg.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gxzuyqcht.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gbjdgsqga.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/ghzqpinlw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gayfzkcyj.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gtioesryr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmmegdexd.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gmtzvophj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/goqkfmkex.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gqyidtllf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gcocltwqm.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/grljgvoqw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gmdgiezbv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gvumkjfqp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gqrjlzsov.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gcmctnrdm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gjcbdiwkj.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gkeafwdgs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqlfxstgm.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gflwbsvbi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gmmdfloll.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gymcrswbk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gymyhihba.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gvagcvkrg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gzkmraohn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gnjgojtua.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gcoxzyxmf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gotnvvsnl.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gpljrcriv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ggldqxsez.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/ghpfwzxdt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gfegdjfwu.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gupeaczym.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gyielsexm.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gzkpcyhle.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gtfallvis.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gzimmgayp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gvwexznlo.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gblvthmnx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gpxpmlgdx.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gqylfgpio.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gefgxpxjb.sHtML


<!-- 参考信息 -->