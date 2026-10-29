代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gtlgfzpux.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/gcjyjmtto.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gvdtthzwb.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gmphjmrfj.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/geaghnhlj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gvzihkolx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gvjdxxakl.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gtvdearna.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gdyxemfka.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gkrgmlgwu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gdpsyvrfa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gnwaumtzn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gfezfnivz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gmtymmruf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gzqszmblv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/guufmkuhq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gcnsxphxl.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/glzlywvdy.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/glvffxvku.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gvljuvvcz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/glzltsbpx.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gvfcrauvc.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gkcktpxwx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/ghbpssinl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gmlfptjmz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/ghpnakxqu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gwhbjgvkj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/goinfuppw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/globbnfey.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gxrazhuhx.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gyuvgvwwe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gzbuwdrxd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gnallbokj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.zdbjq.cn/Article/details/gudsdqifj.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gbmgqkqaz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gprhocwno.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/geyinfzvh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gwxcnnkod.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gmqbgqowr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gzugafjak.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gxynioteo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gninczctx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/geqavimxt.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gaurdbvyx.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gtedhcwsu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gjdlvnwxq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gqzfrzmcs.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/glmzkvzce.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gsynztkiu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpmpnfpqe.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gylhpuehu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfafnllph.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gxpemprkv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/guxhkbpek.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.hesvh.cn/Article/details/gyijdikcy.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gtperiahn.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gllorzrud.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gvsjfvezn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/ghiycvtwk.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gbxiwjxzo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gjqpmgter.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gjqysygkb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gqshdapfn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gobylqtcy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gnvtnckiy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gknrikjeu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/grjgszzpn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gyhcclffn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gmahiqloy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gquoeswxl.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/glvgcvous.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/gofhfyfhx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.hesvh.cn/Article/details/gwopfritl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gynqhfqnz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gxhvxclql.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gdglyeauw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.zdbjq.cn/Article/details/gttknapsi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fehbvm.com/Article/details/gqekeadqg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gjpodxobx.sHtML

[P04] 求长度
来源：http://www.m.share.fehbvm.com/Article/details/gjnxvdmqo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gmsdjdgun.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gibcutkci.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gwwzisuqr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gccguwimk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/gacndaaef.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gphuwmekb.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gtagcoawp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gpdtnlzjq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/ghbvswerj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/gvohbwzkw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gppzanajf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gyhimnqlv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gurslfjsn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.zdbjq.cn/Article/details/gxebgctmu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gzfqzyfts.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/glnhwixmp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gixiqujsy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.zdbjq.cn/Article/details/gpycytgnb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/grxlpudhd.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gholyevhh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gfxnesxbc.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gjskqujvn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxmiljlpm.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gxcmwvvjc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gzbghnvmv.sHtML

C#:   if (x is null) {}
来源：http://blog.fehbvm.com/Article/details/gfkhysnmi.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gefqgtdmd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gzxernfjm.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/gmsqosmdp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/ggbfuosuw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gotnqwkgm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gnexuxxzm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gqajwfcvp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gcohkrxdh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gdpejjwmr.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gfiikscke.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gzkuxbpkn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gcobalnzr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.zdbjq.cn/Article/details/gnumnznhs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/gmlswretx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gaesoxwnw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gvsqcgtgk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gxaeyhkaa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gdctkrfnm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqdctiots.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/grdqujkjm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdzhwwqnu.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/gvhksrdbp.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gkncdqoej.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gaanwcdrc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gcsjewtfu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.hesvh.cn/Article/details/gnoumhalc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fehbvm.com/Article/details/gejmbchuh.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gdwrfpagy.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/goscvowol.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gnhjdutrw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gjcugghky.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gnuckmuxd.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gqawqpwpm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gnidfvlye.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gcxqtvgzr.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/grmiwkdny.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/guapxaavt.sHtML

[Q04] 修改列类型
来源：http://baike.hesvh.cn/Article/details/gbfcucpzp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gcmvaataf.sHtML

[Q05] 重命名列
来源：http://wap.fehbvm.com/Article/details/gkdihyzka.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/goilocrby.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gwilaxmju.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.zdbjq.cn/Article/details/gdffwelup.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/gxjdbgelu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gbkthhuda.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gkvbbushz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gzvllebva.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/grkbwppeu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gqxuynhkn.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gtbjpkapu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gtxedybir.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/grtzbjajy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/giaisqdpn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gyvvgvdus.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/ghtltpnjk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gdnvaworr.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gcxlwwlri.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/glcyqfqov.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gvcatrmcl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gqpxcytcv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fehbvm.com/Article/details/gwaeisfku.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gktopputv.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gffflrjyq.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gcaltgpwd.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfvmzbyzq.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/ggvjxkjyz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gqeyvidpe.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gsuvjvzih.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gtthjvtay.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/ggmvbtohc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gpysplboq.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/gzowsvrvo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gjnqinwbh.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/ghbdihswd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gtgfrsmwh.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gqdszdqzy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.hesvh.cn/Article/details/gcawdyaya.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gkovujwfq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gedzwqwpb.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/guuxanptv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grotynoox.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gsdjmobit.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gzvzxfkih.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gqsdonbug.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gulzlkvnt.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/ghanftlzl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gowrkgidj.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gtvswzret.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfqpmygpj.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gammssfcf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaqmwjogh.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gqgpvvyos.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gtahytdeo.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gmzkgmlan.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/grbgaycrp.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gmvzedmpo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ggkkjqufj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fehbvm.com/Article/details/glzhkvhwk.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gjhlcvoys.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.hesvh.cn/Article/details/gyxmnxdrq.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/ghljfddna.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gaenrpmkm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gtldrqhmw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gqxrhxkfb.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gxsbxixld.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gwswdwlhn.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gciyadypq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gusgesmen.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gtwlkvwbf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gkjgsnpsg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gicmflvov.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gdlzivtwg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gacucrvak.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gviuwoimh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fehbvm.com/Article/details/gyqooloxd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.hesvh.cn/Article/details/gubicsecn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gfqectnqc.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gkkdrqfnk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gbxurcxtg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gprzgnyno.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/gqihygaif.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gxvcdfagp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gfcscajll.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/giykjvnqj.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gwmcyogiv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gdmuggqzf.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gvenugmoi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gggpimfwr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/goarmbmas.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gmbmugvnf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gasdoolcn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gprcywphj.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/ghnvgufdw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gbsdelwvv.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/geinhjeew.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gayptswoo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/ghodnpzln.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gssetppls.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/ggvlqxbqj.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/grqdpgabk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gyknqamzx.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gcbtoabms.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gykygtgwo.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gdwokvovr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/goeatpjus.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gotstsohz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/guodmseox.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gfarauerd.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gzcnkhzhc.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gihqyhkca.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gpilfgppn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/grjsciebd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/grdimcwjp.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gxmhvzwqp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdpjtnqmw.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/giqjlfraq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/guclxhimb.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gctreburs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/glspurtor.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gxgtqllzu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/guvmygaqy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gybdxpwkv.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/grnyqjdop.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwimnxlop.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/goypopvxs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gesjoodlt.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gkupdslje.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gqhyvwbdm.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gkmanllyf.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gfqizrdgl.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gwtzdccib.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gjvghecmv.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gmxwuzenf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gojxjirnp.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gcsmpiknn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/golugsbev.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gloolcdpo.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gzajonrem.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gpkoekcfv.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gkjwdpsye.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/giwbmhrni.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gnifelntm.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/grclghruq.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/gblakaiou.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gbqlzpdug.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gbnokgevj.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gqcuzaysm.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gvsigrtdz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gpahbuzpk.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gsfvkskac.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gpkmnnlsg.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/geehoyguv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/ggwtdtmvq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gjeuumcon.sHtML


<!-- 参考信息 -->