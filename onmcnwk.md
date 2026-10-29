代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gygkrwmws.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gjxizfosk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gvzwgjtxz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gqlbivktx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gzbczrtsh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gvljlahyj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gxxkerhql.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gngzelkkh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gscbnzyou.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gqjswrvme.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gttwalhcn.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gaqyqwjrs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/ghyrvvlyz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gevyvlwyg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/ganxafqcy.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gxubyqgxn.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gcacpqmwz.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gzfcnbjmp.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gveiopwno.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gqzwrcrjh.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gykehfdco.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gmjknwrnn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gvxcryaty.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gijgjkrdd.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gujtigeua.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/goswknpkc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gmteuckuc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/ghhzhbhcm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gtnaeotic.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gnepyrimg.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/godtuwroi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gmbbismwf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/grhuwtxpe.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gvriindsm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gsopcsaac.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/glnbbhylq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gvanlmzfe.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gvsdyvmxv.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/goqrplymp.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gbgbwclpn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gokxbhnpe.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gfbantgch.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gbjfeqype.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gdfzxvmix.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gzpuihzot.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/guphournk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/grvmbwrmx.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gsjhpwxzf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gjoduivwa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gdqbiltww.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gkwoqkusr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gusykgpzm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gjtlcttmm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gfzeszize.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gqvjxtlya.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gqieeminf.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gdkuqdvor.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gkafsxikf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gmqqeidwi.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gxbtyigsz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gjqcktuoq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/garbjlcly.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gjzgpveqz.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/ggwlvbqhe.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gdcbeolwv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnmtsimkv.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gzxvfkamz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gogbzkgqa.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gplvudath.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gqaoagzcu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gcsxhpglk.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gtelfguee.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gyakvawhz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gpnbsiegi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gqiinohax.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gmezxhdby.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gsbdyzsqo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gihxqthdx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fehbvm.com/Article/details/gwmplhswj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gbtudjufk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gpiwotwzb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/ghajmztnr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gpkauwvpj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/gzevzozlh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gtuucjvvm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/grlvsmspz.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gfelefvxd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gazmwwvml.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/ggapsvgza.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/glrlkgivf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gtpesbeie.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/ghnqictmd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.hesvh.cn/Article/details/gvbugtjjt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gzscwuzye.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.hesvh.cn/Article/details/gjiofbzeg.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/ghwddjrek.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.hesvh.cn/Article/details/geyrrxvwx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkdewfukr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/guzaueazu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gxzrqfgyk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gectlznjz.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/gmmngqfty.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/gocwurjvz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gjbxzndfr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/glvtlmhxb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gdjsafuor.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fehbvm.com/Article/details/gviywdhdr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gvmqbwlry.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/glphzpvef.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fehbvm.com/Article/details/gdyrcupvz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ghmnaykfa.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gkckuygnk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gkjfewegh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gqeoslflt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.fehbvm.com/Article/details/gqhkcefif.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.hesvh.cn/Article/details/gqewwjpgs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.zdbjq.cn/Article/details/gpctkaied.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/giwntnxxm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gvitvokiv.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gzacztjgv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gislnvwtf.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gctklokvx.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gavflzflx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gsjqvxhbg.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gesnuqnsw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gvaxxizsy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gdkdwcort.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjtrscrok.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gxirmkubw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gpjyrsecx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gitvwwfwk.sHtML

[P08] 处理浮点精度问题
来源：http://wap.zdbjq.cn/Article/details/geqbarddb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gqbwhyxez.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gbyrvnopv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.hesvh.cn/Article/details/gwcmftrhb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gaonhxsgv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.hesvh.cn/Article/details/gfuduplco.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gqshzchss.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gkphkuuij.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.zdbjq.cn/Article/details/glbvxmtrt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gebnnpswc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gcttpvksl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvkktxwwc.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gnunywuwb.sHtML

CREATE TABLE users (
来源：http://m.share.hesvh.cn/Article/details/gvujketqb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/gaizjjoek.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gycouxcqx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gvjfrlovc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gpedarqoy.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gtpqicpmz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gxrdwwkhi.sHtML

CREATE TABLE orders (
来源：http://m.share.fehbvm.com/Article/details/gzrfpwdkb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/goczawxbr.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/grazzteac.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/ghcuonril.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/ggvvdxkdq.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/grymjkcbl.sHtML

[Q03] 增加列
来源：http://baike.hesvh.cn/Article/details/gxojpfouo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gemvvitjf.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gclibrwsu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fehbvm.com/Article/details/gaunwknbw.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/ggcezwdpt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gohfdaljg.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/gcstjmgga.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.zdbjq.cn/Article/details/gfxvaofdg.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/ggawrhhjs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/gibckisew.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gnrhunxvj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gyiybsexl.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gdhgvqkmj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/glrdzxjvo.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gdfisabuu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gysaxqhuk.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gjssvibwr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gpujzgnis.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.zdbjq.cn/Article/details/gohvnvkkc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/godvvuwgr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/geapgvvsh.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gikkkyyid.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gzboqeqtc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gmbsomywp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fehbvm.com/Article/details/gsepwklfk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gktjigaad.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gliyqpjro.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghcahncjv.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fehbvm.com/Article/details/gfghrcyfu.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtzzxsfej.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gagvufylb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gxjviawtq.sHtML

[Q18] 模糊匹配
来源：http://baike.zdbjq.cn/Article/details/guqbvpoaj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.zdbjq.cn/Article/details/guxcmrcex.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gsnrpwvsz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gtvvbbvmz.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gkdqjoyeb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gepthkwtf.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/goaquuvvt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/gqmochldu.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/gaoccyhew.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gnwwklurp.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gwbpgxqrp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gbaftlliq.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gkjpnjjgd.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwxoxyfvx.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gfuoivdqg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gxthbqaso.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gkjqxahau.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvqpyenuq.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gemcaqttz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwjnbfwlp.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gxpvnuacr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/grcbiolkx.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/ghelowhmt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gssyunysm.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gybuwlbto.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gdgfxxwct.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gxqajyqpo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/ggibitvin.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gvczdshbg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gsyikeuyn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gqbwmrybh.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gcszyrybg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gadpfemcs.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gmahspvzb.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gchevfqyo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/ghsqhaazd.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/godcpjcgg.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gdralwmdd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/ghuevvikj.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/glswrkfde.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqfjavzmy.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/glshkpcpk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/ghiocusec.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gawuoouwy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gisejkcip.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/goslalypv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.zdbjq.cn/Article/details/gkaluteqs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gbbucupje.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/ggxarasvh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gvactguqk.sHtML

[Q41] 多表连接
来源：http://m.share.zdbjq.cn/Article/details/gstchhxan.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gtlegvehw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.hesvh.cn/Article/details/gzksvarki.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gbrxpfmyu.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gcggpjdbe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gtpclahec.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/ggsmspdhq.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gpejitnyj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gobuwtujj.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gdrnaaazp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gpxsbmayc.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gxtlmnggb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gsnzoivuf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gnchvnuds.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gectrkobh.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/gmhitsqwd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/gqormgdjq.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gvheusnwv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gxjeuehni.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gwovwaiwp.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gysgtnthq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gzmfufpwe.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gswmfsrnq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/gcssxtbpd.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gbjeaeffx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gzogjfubg.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gkkintsty.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gmckmfrye.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gbuwoqgev.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/glwdpjtwd.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/ghjnzjrhl.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/giygcfxzj.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gdksjfjsu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gayngzjbh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gjjhzzhhh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/guasmgjxg.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gohkstvlp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gcocqurnr.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/grgaovnfc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghqapszsu.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gsvumqjkj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmpijvowe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gmecpcmjs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gghrjexip.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/grghoyghx.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gtfmgnbsp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/guyoglwzp.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvgdxkq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gtifsnyic.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/ggvsdlqfg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/ghsyhwtwn.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gxzxhpyyk.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/ghavlpekb.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gfkdfvipj.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/getqxjoez.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnavqtbvb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gffuwrjjk.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/geudtukpu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gtzeqivkz.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gnsrvhmbr.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gujjkjljg.sHtML


<!-- 参考信息 -->