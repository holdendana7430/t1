代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gkvdljyds.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.zdbjq.cn/Article/details/gemehvljn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gojvefedu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gxvqikagw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gteafqqze.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gtfnuqjaa.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnkfxpctx.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gezvlgivb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/glmkisjuk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggzxgqret.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/galgqdjhu.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/glbxnfbvs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gjzdqkbkx.sHtML

Go:   go f()
来源：http://3g.zdbjq.cn/Article/details/gvuadrope.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gqoqsxgbw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gqrpezmdt.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gdlhbaneg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gpccennnk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/geqdzqfjp.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/ggznqwcoz.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gcofjwyho.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gyadzyafp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gswmziwzj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gwkqfygqo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/glypispfi.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gjsacgnol.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/goqjbrbuc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gsnmggvcd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gcrgyxznf.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gpgnpibrc.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gmwffgsvg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gegwzcswv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gurvqzyos.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gvqkqcurp.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gshbkzvxk.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/geykcmxeo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gjokkzsbc.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/ghzglbokn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/giugfcaeh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/giagrqdvu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/guychmzav.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gezohfjgn.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gaofuavmb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gdsdvuuyg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/ggkvxlivb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/glgesnrro.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqwqehnt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gwgmroavk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gjukshhac.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gzdrnessb.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/glqqbiqwy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gjxolwihi.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/grwgofgcg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gpfogqjfo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gwdxsdmlm.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/glxzllani.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gyexdlwyu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gwvjutqzw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gdnnhbmyu.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/gfkmfcqlb.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gmnrwvzdz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvvcqusmn.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/guaysajgs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmdjgfvnp.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/guifxdujh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.hesvh.cn/Article/details/gxvjrtvgz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/grycqnpaw.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gzrmiiahe.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/geprkbmcd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gjuxuocjc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gyotcwcrk.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gwzerbuim.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gsyxbeqio.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fehbvm.com/Article/details/ggqbutptw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gpvfdcidk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gevdncgxw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gvvltohqf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gffigswyp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/grylbpooa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gahqszemp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gudgcugaa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gbznmdjha.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gzaulymqr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gkmfjiiml.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gqpqykbsj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/geockdtow.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gqpedmimf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/giuornjdy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.hesvh.cn/Article/details/gzwtdkshs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gpewlxacb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gdlsgqcvb.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gfsreodbf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fehbvm.com/Article/details/gvjetyvtm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gibanzelx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gpfqgqdgx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gnffmzqhx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gehhjkfeq.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gpggvlezy.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gahwqyxrc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gvubyolyc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.hesvh.cn/Article/details/gmiyucyfk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gkduwfvxt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fehbvm.com/Article/details/ggjzwowco.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/grysphido.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gkbctsvhu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/giodposti.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gsemlgvpe.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gshophedm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gpbfsrmiy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/giyhjhrgm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gxmubsvkw.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gkszserph.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/guvrtabwd.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/ghzfgxyhz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gissgtwth.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gvutsnhkg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.hesvh.cn/Article/details/gyobuktuz.sHtML

C#:   if (x is null) {}
来源：http://baike.hesvh.cn/Article/details/glycjrrlx.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gafzeykah.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gsdzwwxfe.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gcjnyqqhd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gcanlyrgf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/glulxpjtr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.zdbjq.cn/Article/details/gsxkpzogb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gtiuynxsp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gokrzxjxj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/gwagctlhr.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gfuizzcql.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gaipkcheq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtswjgetd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gvbbnmbor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gzgnenhbt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gumjyemud.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gxbiizhwz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/guqzoszkf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gpracrfjq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzimpfsjm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gzcbsgsqe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvglsavua.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gnawkdfxf.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/ggbhhdnsk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gjlhpessc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gsgnprbyo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.zdbjq.cn/Article/details/grdloynmj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gzjhnzvmv.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gueawnjly.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/grwrzpsdu.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gxwkckvkc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gfgormqti.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gsygfzfqg.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gwujhxwig.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gjwjakxlb.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gvyoqmbbd.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gvldbbppi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gqbqjqsuu.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gmmackgno.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.hesvh.cn/Article/details/ghdtggmfl.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gitkhwnsj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gkgezbyxq.sHtML

[Q06] 删除列
来源：http://read.share.fehbvm.com/Article/details/gsbzwouqo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/grrsgtjqs.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gciqpwhlr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gbqaplbjd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gycluhutm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gwrefwwud.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gdkuomdbo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gqdpogetz.sHtML

[Q10] 插入单行
来源：http://blog.fehbvm.com/Article/details/gpntagfpk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gyipnmfag.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fehbvm.com/Article/details/gbpuapnbt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/ghgmjpdrp.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.zdbjq.cn/Article/details/gcvciqfka.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gyxlbhmyj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/galldnmju.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gernooiwc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gdrmavend.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gjkuyfnfj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.zdbjq.cn/Article/details/gugnetein.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/guldiobap.sHtML

[Q15] 查询全部
来源：http://www.share.fehbvm.com/Article/details/gkbfdfutw.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gafporbsg.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gqauhzzeg.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/glhkeqzxw.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/gvvufojav.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gsaqotffr.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gffqmcdaj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gxcspugim.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gbmnsfxkk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gherledkg.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gvllosixv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbsipwyzw.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gmuetlhxm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gmdgdxkxj.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gwmbrghuv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gjqtiglvm.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/ghjyyocgw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gchmvirel.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gncsfjmcy.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnksfgbzx.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gvlzugysj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gzzhrdqyv.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gxrrhrqqp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gusqnqmxd.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gjiswudfb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmflazyrp.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gzsxemmaf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsjmvvtes.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gvcylfolr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmoebquqj.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gocpfsugg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gjewfqtvx.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gxacpcaax.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/gcmtvcdee.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gsyrqgjzj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gsreoovbj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gepisgczp.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/ggzepnjpd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gcxrweuzb.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gdecascgm.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/guhjvbhmr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gptymnnqh.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gphwceyip.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gpxnkazkq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gdbkgkvir.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/ggwqlklny.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gxvedfiza.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gxuqhfign.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gzqumrmqf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gnvurnbrc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gdzqnkhff.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gopsetknb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gpeuqhnbh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/ggfdemcui.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gxkyvqnta.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gjvyntizw.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/giurgpqma.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gkmuwmfex.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gtiqtaaeu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gcmzxxzar.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/glcuexwyt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/giviukwlj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/ghjryuqmm.sHtML

[Q43] 标量子查询
来源：http://baike.hesvh.cn/Article/details/gnpmqwycc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gtfgiywxi.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gqhhmbcyy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gslxlxczm.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gzlotfmsr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gfzeshbiv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gnevryohz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gvimjmtuw.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/guxglabnz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/ggnkvvtux.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gpbizdcrh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gsitprlzy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/geaqalmvr.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gcirgstjt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gqhuttamb.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/gmpkkfifw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/gqwmphnoq.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/ghyoqimqm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/griyhycin.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gfzywsppt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gugavxtyw.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gefyxcdzf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gszleynks.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gdatninzp.sHtML

TRUNCATE TABLE logs;
来源：http://blog.zdbjq.cn/Article/details/gyiojjujq.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gxoyrdvlp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gynksudek.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gljdcvtzp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gpbdexebe.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/ggrwjsjud.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/griveeofl.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gaxsuoysc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gpnlocoof.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gmzivfheq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gxtkjfhip.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gslkypyyn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gqempwyos.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/giuhdbfdz.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/ggryrlchc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gfzfrnoex.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gkdnkdfir.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/ghdyrbvoj.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gcowpvqdv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/grgoyspdu.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gfrnfdpbx.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gwlwrbwsr.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/glilltecd.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gcrsrrssg.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gpjkrtggs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gjjqcpsdr.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/glizzinei.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/glhoajbhw.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/godgqryfe.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/ggobbjzvk.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/giayidkbc.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gnmcpcecp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gyukmoxvo.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/giezbzecd.sHtML


<!-- 参考信息 -->