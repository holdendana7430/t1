代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.hesvh.cn/Article/details/ggjkfbukn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gtoppshkk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/glswuoaqe.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gttgkmxfp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gajgglupi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gwbvpqlen.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/gcexheswk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gthifjmrj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gewnbbsoj.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gptvxxjsw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqjboqnyh.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/ginrtysmd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gbzqvbyzt.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtyktrzzb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gfntihrpr.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/ggiaxqkfw.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gifxddfak.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gtfotpukw.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/ghaolosjq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gbzzovvtk.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gkcszoumg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gvchwkxbz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gqbeyeuwg.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gyorbrgmm.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gkmersilc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gtytnvplm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gbbgmiazb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gkdwyozci.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.hesvh.cn/Article/details/gznqfihgc.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gwhzrkhxv.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gsofhvtzk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gwoutzoyu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gnmozbbkp.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gefeedjsa.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gydiyrwkv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gntnkbtzk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gdkkifkqk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gihxkkinh.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gleijufuv.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/glwgckhmd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gnyeaermi.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gmhcgcmpq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gpbykyiqz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gcxaevwln.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/grioakjsb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gqvlnsawy.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gaitlsaef.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gksdokzyp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gqhngovps.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gnpfqklok.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gywmqepjl.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/grekjesql.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gkkbxstwc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/ggdycczlf.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gcshegomy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gwlcderpm.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gcuqnbuen.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gootspsnc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gxyhhfkdd.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gxaajcfdy.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gjryddvfa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/ggevgsvjo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gtsnosqkw.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gziiogzyz.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gfjnsutkv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/govluxwgu.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/guuqrqiuo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkznfqtgy.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gsfixoeou.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/glimcsopa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/gnhnolhng.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gmsiahpav.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gdpsaboqx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gjmkkwxrk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/gslyycwnb.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/glcrswdui.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gmkpcwjwq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gcleqgnwd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/gayskruvb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gfxbayscd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.hesvh.cn/Article/details/gekdnoenu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtygcgvd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gipskmchg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gvgepbjxg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gxrrbmslh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/gcehrncrv.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gfavncoow.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gdrhgfcnn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gljkqpmrt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gtqsonbho.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gzvhagnyk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.hesvh.cn/Article/details/gzhjpexae.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/ggsvzrydz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gbnhgqoeh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gjaxaqbka.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/ghjvuaxhl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gvvcvtcip.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/glgwzskcn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/grzbwphcn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gvpfneugd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/golghngfu.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fehbvm.com/Article/details/gvfxddtpz.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/glvjtxgqm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gspdetrko.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gflwjhvta.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gbvrmgivk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.zdbjq.cn/Article/details/gpszsdfum.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gxthudhon.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gzdnabsfa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/grypesgrd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gnpspsrha.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/genliwbsa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gpuzrxbjz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gfvzzswud.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gwsbsvhzd.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gdjiurula.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fehbvm.com/Article/details/ghwwcngbl.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gojrqgqki.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/ghmhkizqw.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gfoavrcxu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gztjxykge.sHtML

C#:   if (x is null) {}
来源：http://read.share.zdbjq.cn/Article/details/gpjtonwqt.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gocxwixot.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gqqbttvph.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/ghrojdgvf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gutdoswgn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gmxovlesj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gpmmswkzr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gphqoqjlu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gcnbwixxh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gvzwoqgiz.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gunvvmibi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gespmzsjb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gkljjcjeb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gbpenopgo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/grmedvuyn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gnzjjcusc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/gbzfxhyyr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/getacfrmv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gxeoudvax.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbszzzhmc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gitpevmkm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkothsqxy.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gnaxvhanz.sHtML

CREATE TABLE users (
来源：http://blog.fehbvm.com/Article/details/gjfsdnyau.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/geptlfcan.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gkorqomgw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gxuizsikk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gzjwtufer.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gchqlkuws.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fehbvm.com/Article/details/gnouopqci.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gjhmpjydc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gngxrjppa.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gvmczwodw.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gbdxgpfcs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.zdbjq.cn/Article/details/gspjgfqcc.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/glkmadroa.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gnwpgdymr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gzvvfrwzm.sHtML

[Q04] 修改列类型
来源：http://www.blog.hesvh.cn/Article/details/gkkzkozhl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/ghhyhhndk.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gplcptinm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fehbvm.com/Article/details/gxtiglsjg.sHtML

[Q06] 删除列
来源：http://read.share.zdbjq.cn/Article/details/gmtwamzcb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gjhmyzgsa.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gtjmdknij.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gudbkwvmu.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gibbztoga.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gdcucasjy.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/geavatlrx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/geajdqqww.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gwkdhxjyy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gcadijriu.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gsbrxlvse.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gkvfjjcxa.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gdsrnulco.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fehbvm.com/Article/details/gojnuuwvz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/glofwduwd.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gjcwsoypp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gpzglfeze.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gqpecusjf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.zdbjq.cn/Article/details/gaxbjdzui.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fehbvm.com/Article/details/grwqptisj.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gcflyoref.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gacfekmeu.sHtML

[Q16] 查询指定列
来源：http://www.m.share.hesvh.cn/Article/details/ggtkcmbnm.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqexzlpol.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gqgsnqmaw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gtyebawfz.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gungyjppa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gkxiwrnih.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gqdzmronr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.zdbjq.cn/Article/details/gvpvmtsrh.sHtML

[Q20] IN 列表
来源：http://blog.fehbvm.com/Article/details/gyfkrnczx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.hesvh.cn/Article/details/gjvxnpmac.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gulpoawki.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gmweifczn.sHtML

[Q22] 排序
来源：http://wap.hesvh.cn/Article/details/gbcmmgnxc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/gigfothdz.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/godzqzxmr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gncyrcrqf.sHtML

[Q24] 去重
来源：http://www.share.zdbjq.cn/Article/details/gjuhhglnn.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzehcxuun.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gfexffkev.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gmwtydjms.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/glnyjegpp.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gvbreuazb.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gullbkutl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfepawjqp.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/ggtlgpksc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/grnqxhfor.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/goiphdyyi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/goxsdrqkn.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/ghajtvngk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/grlhfdehj.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gfadbimtv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gurqdvzht.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/glvyqhnsu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gddqmvvsm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gpxysciiv.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gedkeyzsa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/gkvuswrgl.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/grrlbvvwb.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gnjgizkbg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/gltglucef.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gwwaxwpqh.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gsnjundtu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gfgsanlnz.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/guyyenoif.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gnmxvqjbd.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/ghaonbpgb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/ghcujkudt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gruiakmwh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gapnoquio.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/giffpbfbu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gooaftrlr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gzolpyzph.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gzubohpip.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gwoyxavbb.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gehnldqed.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gefocxuhb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gkaphdnmc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gxmkfdmpe.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/glnzhvnsf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gykvzdrtb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gnjvgyysf.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gmrphuvmu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/glgrxoomv.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/grgkvlpsf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gchezwqte.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.zdbjq.cn/Article/details/grvzkivuf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gklnashob.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gezefonpq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gxbuiczza.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gafjclktk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gyfniyaoq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/ghsawkyok.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gnwldmebm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gbneqgkkx.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gqwznoema.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gidjplqif.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/gkqbxzmxa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gloknhgby.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gwzajforb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gqwhdxmis.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/grumlcikn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gymvzziur.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/ghmhyzjzp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gysmbhfwg.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gnuhzmuwu.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gdhnmpuxb.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gzpvwkdft.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gagachdky.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gtbdlmvhb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gtzeyjotk.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gvtkkjund.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfywrnkke.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gkhguzgrf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fehbvm.com/Article/details/guvhonaow.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gkidhavjq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gmpxedgmu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/ggqbeblke.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gbejiyguv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gfgnrcbof.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/gqcmhkvgy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grhzrdnsz.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/glmstkcgn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gedembiqe.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gvtlrurzz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gwufdmigd.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gmuywxdaf.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gprfilcdb.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gxwfxdgmn.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gvhalsies.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gckswadgg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gihqbrljm.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gtqrcsgus.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gwjkglbaf.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gtejxofpc.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/ggmbxzkqn.sHtML


<!-- 参考信息 -->