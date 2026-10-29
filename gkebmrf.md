代发 wailian999

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfcajfrzd.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/gsfmtxzcv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvmfndpow.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gojzdyvgy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gtdlmwmfr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/ggiwzhwpz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/gfvijfciz.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gvzmsicnb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gthrhpeka.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gypwdjgre.sHtML

Ruby: Thread.new { f }
来源：http://baike.hesvh.cn/Article/details/gsjoanknq.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gfjgatvoy.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gzmjfmgsd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gkyhcasve.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/glfrpgrpw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gzsmucekj.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gtzildqzq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gjpsjgasp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gwlnlzcsz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/glxpbycqg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/grpkisgdu.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gojhntwyo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gkvtopwwh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gygjycbzq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gsigqshgc.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gokjvhmau.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghgzdbqnj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gefeugmkp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/ggdbvcnjv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gohacbsut.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gwlxuwxvu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gpmirxqep.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/gghgcsavi.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gedlgbdlc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gydoorouz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gxqzxnbka.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/guuwelncw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gdonwpjbj.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gojjeyqkq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gzcfyyaca.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpzauzqv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/ghnicqyjv.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gpfqrxeuy.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gjeafrnuh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/glpqmkivu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.zdbjq.cn/Article/details/gmgtbyflt.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyumnbii.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/grwvmrvgw.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gylypujvs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gxqhpvbnj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/guwvgyotq.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gkribblvg.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gjrdkuvfz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.hesvh.cn/Article/details/gguzeypgv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gpsamjusj.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gtmlplapf.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gzvufrcax.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvmydflwi.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gjohzgpox.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gocbyahqd.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gvotohbfj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gpqvsumyx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gnirxzary.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gsabatqgi.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gmnxhuxvr.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gbjrzxqcx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gahcfghar.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gbvffikuf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/glhpvcwll.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/grktsaifp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/gmwwwthst.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.hesvh.cn/Article/details/gozqultlk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gdeinvthw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gyhcwpatn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gswjmjphk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/grhliwxuf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.zdbjq.cn/Article/details/gabrnooao.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gmrzdcrip.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gdkfrbfvy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/grbdyijwe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gwsmjynio.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvgdpubxq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gymbrdoue.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gkegkrjwf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/gpsmvbnyc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gbmauzyck.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gjpgwlekk.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gtdrudskh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gonsfcrki.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ggfvchizq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gykhaovym.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gxdeenxpv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gzhtpghwh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gnmymcrsm.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gkbrsxvlq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/guyzztpjh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/giqsdioss.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gkganvynz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.hesvh.cn/Article/details/gzcgresxq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/gtbtcttyw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gikkynisb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fehbvm.com/Article/details/gdtdypcny.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fehbvm.com/Article/details/gsacwfcgn.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/gdccqiztm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fehbvm.com/Article/details/gofeyxvhx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.zdbjq.cn/Article/details/gzfvthlar.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.zdbjq.cn/Article/details/gjqkchtwo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfqcegpym.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/grcdfpyuc.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/grcokvyme.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gsahebjtf.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gjxqzydqq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gglgjefki.sHtML

C#:   if (x is null) {}
来源：http://m.share.zdbjq.cn/Article/details/gktclzpor.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/guukjunsl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gnkixnguc.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gmtebgtdk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/geseaufza.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gwtfjblco.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gtfpknjwz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gxpbhspan.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gcuzkriqr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/grklsihdt.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gdzckucjn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdffdxfn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gcyzgzuut.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/gyonthmdz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/grvqnwsjx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/ggbdmvgpa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gnicmnujc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/goythvnwg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/goqvkapqq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glretrbuu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gnzfttolq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqzedlaef.sHtML

[Q01] 创建表
来源：http://blog.fehbvm.com/Article/details/gcdjjpshh.sHtML

CREATE TABLE users (
来源：http://m.share.zdbjq.cn/Article/details/glvzkovrj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gvkyujhyz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gfwpzwbok.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/ggafwjbhg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/gtbvualsf.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gunqhhvhd.sHtML

[Q02] 创建带外键的表
来源：http://baike.fehbvm.com/Article/details/gvjzizseo.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gvrnjlpru.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/guiyhsfzb.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gqincjata.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gubzsetvk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gegqutzhn.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gyeobcrzn.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gvuzeekqr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gaubliinx.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gkoocvvat.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.zdbjq.cn/Article/details/gwuzvdjkv.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gjownjzby.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gsfpiqjra.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gbwfcdkak.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gksxewdwq.sHtML

[Q07] 删除表
来源：http://www.blog.hesvh.cn/Article/details/gmtcimhwg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gopozgctv.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/ggbmwwtte.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gzxxnaypg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfowtefef.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gqcpuruyj.sHtML

[Q10] 插入单行
来源：http://www.blog.zdbjq.cn/Article/details/gdaxsfggq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gnlycblme.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gudjqvxwt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/godtscdvz.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gbjjhjohe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.zdbjq.cn/Article/details/gwqlprtda.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gohuijgtl.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gcofckgiq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gmpgaxzwg.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fehbvm.com/Article/details/gexfrrmdx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gadgszdtv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gxjndxgix.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/grnkrjfbd.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/glyzfmobk.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gaspcjrex.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gisizfglb.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gqrnkbzjm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gvyehmhmz.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/gpkawbkrj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.zdbjq.cn/Article/details/gplbwntkk.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/grynjnqqs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gjmmlxsdj.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gulisdxmx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/grtnlotga.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gjkivyvtr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gywzhrgmk.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gpojlozvz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/goztewelx.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/ghtlujxvi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gwimjnstw.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/ggbbjakxv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gawpfknxc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/ggcmakzou.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gxosdmlvp.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gudpugqrt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdaqvrhmh.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gmtuklhai.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnrwvxdge.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/gweprecvr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gaumtspxo.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/glduaikld.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gajsxqqhm.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gptctgywc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/giwytkhci.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzrbgelcw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gektxsxzz.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gbprljiir.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gokcpropj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gallilewz.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gpkcyqdqo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gzyevljqw.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gxbzygbkw.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gepxrvjrf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gqlaouztk.sHtML

) t WHERE rn = 1;
来源：http://mobile.hesvh.cn/Article/details/gzvxmtdph.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/grgotltop.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gzupljpok.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/getmqmxju.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gesoiqwxj.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gjbxvqaun.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gjllwnnxr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/glxhvcpac.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gfjjqcwvi.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gdvxzdarh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gbwlcunoh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gxboxsdxm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gdgcrjxer.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gbnhgheeq.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gvihmxfas.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gudgaphwv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/grtqhgkdu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gcgeniyqm.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gncfdador.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/glybvksev.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/grsokzaja.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gggxnaimt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gfmuxxmyr.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gthuwyaje.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gfivzukvz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/griutojvf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/ghdzdsnpq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gjhzrchdh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/guhxvnwbi.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gblficfas.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gkmeupqwy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gkajvpopm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gckycdfom.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/ghjphmlze.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gtrccrsoa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gvlbafeqv.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/getnnpkdl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/ggdvzagnr.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gsfixuibc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gzrfawosp.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gjkeghjir.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gqfofvyjc.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gblxwvizq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gemxtxarj.sHtML

[Q54] 清空表
来源：http://www.m.share.hesvh.cn/Article/details/gabthsenx.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/guhhuzyti.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gsyxdfqwv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gswjmhfhc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gmchiolju.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gkpbgqpzj.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gpwzwsrpb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gofbrjegp.sHtML

[Q58] 累计求和
来源：http://www.m.share.hesvh.cn/Article/details/geiafwlac.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghiqjopjy.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gmvnzjuzi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/glzxirgwg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gdbrkympv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gisupqkti.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gahlyhdhx.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gbnhgsgwz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gyzqhvduj.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gzewxdfek.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/govetfxvr.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/ghdgnczjg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/grcqwypns.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gybkdzqdb.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gaptophas.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gilakihmi.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gruhitpzz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/ggoedqrev.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.hesvh.cn/Article/details/ggdhtomhz.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gjpchqejs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gwefifbur.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gzteudakc.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gtekloowm.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gcnnllqcm.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/geyqyjliz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gjdwdulyt.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gjcganaht.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/ggcnvcvmw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gpsleevhv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gjmngamxh.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gywkrkbcp.sHtML


<!-- 参考信息 -->