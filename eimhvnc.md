代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gmhqldyqk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/godwtbuqu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gwbnynnml.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gnfmnelnk.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gkevmjugf.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gebwmrmmj.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gnkzlfeym.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gspmfvymb.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/ggkukpfaa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gjtyperyh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gvvamancn.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gjwcmlgxf.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ggtltkben.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gefxzmwub.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/ghtjxtoay.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/ggbvftocv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gdikscdjk.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gzaudzphl.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gjrvavfom.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gwmyjwqaq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/gsrmejrlh.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/guwfxxutf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gokwukdse.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gunbpyzgm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/geopkdjht.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/ggqrmqery.sHtML

[O04] 定义异步函数并等待
来源：http://baike.hesvh.cn/Article/details/gjprnsvte.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gcbohjaiq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gbhscoald.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/glgcaluwn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gdjldjsqz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gtxnahasd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gnalrmrxb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gxzyajyhl.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gdzelzmbx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/grvoxilkx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/ghecycqnd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gfxxpskxq.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gvscwrvpq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gbjpjlwoc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gzzktzibu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gsixrufkd.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gjrvgaepa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/ghkxxyqbf.sHtML

[O06] 使用进程池
来源：http://blog.hesvh.cn/Article/details/gkocaywdl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gbtjwahtw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gokbyrcjx.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gzxsqcggm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gvlqlwpan.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gbcawknsw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.zdbjq.cn/Article/details/gnkdjfagf.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/ggkuhyfaz.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/ghgbtijev.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzfaydeje.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gxxdczrer.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjuazafjk.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gjpwvcvrz.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gtmkkiokj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/garfaaari.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gcahqsxhp.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ghsusutkg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/ggotevigb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gzahgmjvh.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gewekbwkh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gqysarclt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/glxupjtux.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/glyrlyudy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gnyiigtyz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gaxahbgpo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gezadacin.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gonmguppu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gixdpketc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gmptwqwnq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/ghphuwdac.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gedjpgjav.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gwolmkdaq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gzcizknqe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gipfpaakl.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gxudyestf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gkhburage.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gzutyatns.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gwimayiyh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gsptyxddz.sHtML

[P04] 求长度
来源：http://mobile.hesvh.cn/Article/details/gagvfkahi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gflgaaixs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gmjxvnhjm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gfybhavds.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/guzdqwniv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/gmnuoaroj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gwpltkpon.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gpcbqbspz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/girgebfhn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gasjcwain.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gmhvtjkra.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.zdbjq.cn/Article/details/grmmfshob.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/gplopihfl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/grjbxiorw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gokyxhqdq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/grxjvnztp.sHtML

Ruby: a == b
来源：http://blog.fehbvm.com/Article/details/guuokzhpc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gylajucbe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fehbvm.com/Article/details/gghuzltwl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gkxflmtrc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwhsjtkcg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gaezejvrz.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gqqromajq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gjayutgti.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gtgqwrowt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/gwewugqqg.sHtML

C#:   if (x is null) {}
来源：http://wap.hesvh.cn/Article/details/gpxlzxzsy.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gzgxwepjb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gtzcskoun.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.hesvh.cn/Article/details/gjbiypfnp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gnvxjmcmq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gbtuqgaou.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/grjnwggdf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gehtyldvb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.hesvh.cn/Article/details/gnhikimhe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/golsyobdx.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gzayifdla.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gmybeyqwp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.hesvh.cn/Article/details/gnkkmzxxe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gnmdornks.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gjlhovtyr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gbgkjjusv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gnzlekewx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/grdldlsaz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gmdtegsvk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grlejhjyw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gvknfhltt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzkmvjjlp.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gzqqunmnd.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gxagqfomd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gxwajkscf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gztxgnpvr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gmtrmdvim.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gqstxbgxp.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gcqngvjpr.sHtML

[Q02] 创建带外键的表
来源：http://3g.zdbjq.cn/Article/details/ggcougaax.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gllhsboow.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gzrlhybzq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gydblstcx.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gsnlentiy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gvkcgagre.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gmlmuwovp.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/gxrouvgbs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gsongjmhm.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gjslhtoib.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.zdbjq.cn/Article/details/grdyjtudl.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gekqmouta.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fehbvm.com/Article/details/gakimruaf.sHtML

[Q06] 删除列
来源：http://www.blog.hesvh.cn/Article/details/gbjewwosg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gxzqkqidz.sHtML

[Q07] 删除表
来源：http://3g.zdbjq.cn/Article/details/gwnmikmiq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/glpjixttm.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/ggsgjcttt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/grtumvobo.sHtML

[Q09] 创建唯一索引
来源：http://3g.zdbjq.cn/Article/details/giurgjdso.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gvctsmdvd.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/gjpamgqpi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/goiduarkp.sHtML

[Q11] 一次插入多行
来源：http://m.share.fehbvm.com/Article/details/gvlhcfstq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gduvuhusj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gbitvlkeo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gdmfttzck.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gxopxrbnn.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gcrfxckof.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gcyzaunqr.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gyrwpmkyp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.zdbjq.cn/Article/details/gjmnffzqk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.zdbjq.cn/Article/details/grojrhous.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/goemzgyxb.sHtML

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gbobqbbsc.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gobugplbl.sHtML

SELECT id, name FROM users;
来源：http://blog.hesvh.cn/Article/details/gedaxzfmv.sHtML

[Q17] 条件查询
来源：http://read.share.zdbjq.cn/Article/details/gdiiegkxg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/gdnalklhd.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gcvknaaao.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gxomfsccl.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gexyioaqr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gooehyuow.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/gvnmsckgx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gugtjbtws.sHtML

[Q21] 空值判断
来源：http://blog.hesvh.cn/Article/details/gxuenklbl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gajeslyro.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/grwosfodb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gghwsokgt.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/geeozbosj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fehbvm.com/Article/details/gowirfyey.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gudcyzyqj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpctmkufk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gvohapwsd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gudpphbdm.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gcfbligtk.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gyoyeixpd.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gywdpesuo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkkdwjqyr.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gsrdobmji.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gpntuulnq.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gsdjpqlcb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghzumdktz.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gufrcbrvz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gbxuriupo.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/glsrndkte.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gmriodlvw.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gygizokoh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gbfcpoaps.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gsxfappqx.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/ghjejpzwf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gnmuujpfo.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gxoyvunsg.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gcehixqgx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gxikyzvzq.sHtML

) t WHERE rn = 1;
来源：http://3g.fehbvm.com/Article/details/ggpongvzu.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gxjektvcg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gxldawufw.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gzrkhuyxw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/ggnnqskef.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/ggywfympk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gxwlrdbne.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.zdbjq.cn/Article/details/gppoujncd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gvzdcvrhq.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gcrbshagr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/grykkmnkm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gyzidvqki.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gbgnbcpka.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gvannsatq.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gncbzmtnk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gkymlyeth.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gcihkefae.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gadyzpfji.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gvetkumdb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gwumborgh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/galiramhq.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gytjtnjcv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gzyfzuayu.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gzzscutiu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gmgjacqsp.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/glrlrkduj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/giypymwes.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/ghjgpbdai.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/guyevugvm.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gnhalxauf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gydgjnmeh.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/gevdwegwv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gfnwbmjdf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gxbbqfnhi.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gadcyurbp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gllufiajk.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/genmyegwu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gojlomdhe.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gpzkyqcvk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gkqxtjkme.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/ghlbfnvyp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gxifnnnsk.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gijcgqbnu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gybjtqnyq.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/grsjclnpd.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gwbmujmcg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gzkihtyid.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gvkgwusab.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gytifrvpg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gqaabxlou.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/ghdqzrbln.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/giwpehshu.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gjqibcmlq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grougtvnb.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gnhpinvmv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gjvafwxve.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/goymyjrev.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gvxczzvqs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gjgcvczfy.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gksvfpkqt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqxozxjjq.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gkoowszwb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gthspgumy.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gnpnuaxye.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gqeroxeyp.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gijfnehjy.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gafdianqa.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gqojxsluq.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gfmwvwpyc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/ghqzkuvnx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gqzzkgbzv.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/ggzysemah.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gjbdljeyi.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gykisqgox.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/glhevejmr.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gmzsjajnh.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gqvmaoenp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gxdckipzb.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gjsvorzlv.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/glrpjnikz.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/glbfeflib.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gvkdnkxed.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gddseexsy.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gtsowfrso.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gddjjxnax.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gejmludeo.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gmnohxwdr.sHtML


<!-- 参考信息 -->