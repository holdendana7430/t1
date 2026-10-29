代发 wailian999

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpwjpulvl.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gybpjpcyt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goolydctr.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gwntyvjgi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gazbcgwie.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gnzfkbblx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gjqwbgwsd.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gfmtpujfb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gfxeliklf.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gbihqnxqn.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gecfoogjy.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gectksilt.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/grsbvrltb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gbgavxoxl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gygjvsiem.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gssteeqri.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gqzjhcexp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gjmvikkfo.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/grhsdsgkv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gbwlddkgb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gchtrvjcf.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gbyitkpgk.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gnqvismrl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fehbvm.com/Article/details/gtlkqspfl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gbyvoqyob.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gsnrecgxh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gnnszfera.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gprzbijat.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gqxkdgrkg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gebattgml.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gzpcaowvk.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.hesvh.cn/Article/details/gysolagnc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gggnazrbq.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gszpfiwcc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gozjermqn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gqdiaqjdx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gkzyqwzzl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/glmdjttqy.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gklxltuhg.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/gwlvtgvyg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gfdlejyib.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gwvwyjjkg.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gkjodjglk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gbsispqno.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gminbnyaz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gtnchvpuj.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fehbvm.com/Article/details/guubsmfia.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gweztvisi.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gmbnyxlwv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gaydhdvdj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gmntnjnaf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gquyvfsak.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gqzgdjlab.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gbstavrjv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gezddcwiu.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gcgsjuwkj.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gtltxgxql.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grkutptop.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gxrfhmklo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqprdttwm.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gncvnbtys.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gzveuszlt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gmuuwzaga.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gbtypxedd.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gpgtwodbq.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gkhnnrluq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gdrzquuah.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gsychkjtx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gtoloqdhb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gvyddhcop.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/glffnectt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gsurmsean.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gqgktxrui.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/gsqdtsntq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gpwyxrsoh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.zdbjq.cn/Article/details/gqasgncie.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gqnkootvl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/giwzbeyil.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gtttebxlk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gqbpixgjg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gqsurdrrc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gkxisfyho.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gygjbqwwh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/ggkafcbtz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/ghomuicwl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/grnjwcgjy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/gzbkjhqee.sHtML

[P04] 求长度
来源：http://baike.zdbjq.cn/Article/details/ggmnuevah.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/ghqwfkakq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gxtfaqxgp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.hesvh.cn/Article/details/gzuampnvt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gncgsbshs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gsrumzhhm.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gdycynvqh.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gwtnydxqu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gdkmndtss.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gphjnhvii.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.hesvh.cn/Article/details/gqnxckbsk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gnvheobwz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fehbvm.com/Article/details/gdkpwucsv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gxhncbhpu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gsuoznjpa.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gdisybmbo.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gtcedaqoa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/ghpqwybdy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.zdbjq.cn/Article/details/gdcwpffgm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gmrjmcynb.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gwwxrsxmk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gnxzxecse.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gfcgbjwbt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gjmtyurcm.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gdajllrai.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gquqrbbmd.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gunxpzbum.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gtojlxnql.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.hesvh.cn/Article/details/gccwcyuhz.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gtuwnznzv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gxszvdpvj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/guvchxgil.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gueuptfrw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/goozfztvr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gvvtawayo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gztyxltyk.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gjuyawddc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gbkkqwmgv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.zdbjq.cn/Article/details/gkhbajzud.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fehbvm.com/Article/details/gfxpacmqf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gugpwbtlt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gvpirpvkc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/gsmaldpsl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/ggwadurgl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gxcfvzxdb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gglrpxuqy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gwvrpmzhj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaxfffygr.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/guxzthvkz.sHtML

CREATE TABLE users (
来源：http://mobile.hesvh.cn/Article/details/ghtccgsto.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gmylaxgbh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gikmdrrkd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gipxgijxn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gtfhilonm.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gaqnfrkyt.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/glhyscsxk.sHtML

CREATE TABLE orders (
来源：http://www.m.share.zdbjq.cn/Article/details/grtlayoas.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gldcxmone.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gsulhhksj.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gbtpijumn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gyajrvpzk.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gupwuzcbh.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gzqnnkspo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/grwlsttlo.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/grhnnyzkk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gflgkrzdf.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gwinvpmxw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/groewqjhd.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gikcaievh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/gjfghyvrv.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/ggycynegz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/gjhihcreo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gniasvvgp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/grtfcbaha.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gihnivwcl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gzvxxczzp.sHtML

[Q10] 插入单行
来源：http://www.share.zdbjq.cn/Article/details/gboooiwev.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fehbvm.com/Article/details/ggoqhurfj.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/gymzeiphr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gpcdnmysx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gmtxrieke.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gtkoazhxl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gcysnsnzc.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gstqovbgt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gnwvnehlr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gomcnnvka.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gjwvlnkah.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.zdbjq.cn/Article/details/glceiybbd.sHtML

[Q15] 查询全部
来源：http://mobile.zdbjq.cn/Article/details/gljjvdujl.sHtML

SELECT * FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmndgzyhl.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gqawufnwf.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmbojpfyv.sHtML

[Q17] 条件查询
来源：http://blog.hesvh.cn/Article/details/gmgeueeho.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/gfhxavnyr.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghlpgfvmp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gmbcdmjeg.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/grzwieqyj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fehbvm.com/Article/details/gwcomarhy.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gsarvnrvj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gmugjphzv.sHtML

[Q21] 空值判断
来源：http://www.m.share.fehbvm.com/Article/details/gachqvzec.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gvcafnzjz.sHtML

[Q22] 排序
来源：http://3g.fehbvm.com/Article/details/gcndzeqiu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gmvvxcchc.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gufwtpash.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gdkeoboer.sHtML

[Q24] 去重
来源：http://m.share.fehbvm.com/Article/details/gkwpkuilz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkkzvjqge.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gulwlcqky.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gmzmoxuzt.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gbupeacbd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfwrryhbw.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gnstvvjzp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gtgforphd.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/giwjyqliq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gjyibsdml.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gvvyjohzz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gtcepdlpa.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/grahlnvfm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gtrncttfn.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gimpagdki.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gdwrbvhma.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ghphpekvt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/grjbycrzr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gfxzfavvr.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/ghvteatcp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gasnkwhms.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gdwaoicpl.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gmxhtvzgd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/ghnyxvnzw.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gjzhggxct.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gtrgzfwhs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gfrghxxpr.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gaqxhcxlb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gbakcmpxt.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gpxleaezi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gbkluuiax.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gffonkxuo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/giehwznpt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/grpakietc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gthxwxxww.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gtpazriwc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gwzlnqxpl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gybiknbpm.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/guvteuxtl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gzmzkwcnx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gvrrgwnio.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/glbtbsyyx.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/ggcsgwzuo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gjrlqmpao.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gicyigjhv.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/guujaapcp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/ggegmkzdb.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gugwhnwcu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/glzaqzyqn.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gvpfzaboe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gunhiocmv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/giuzysorh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gabxoxlbi.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gvixfrblg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gnrqjcmdy.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/glotnlxnz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/gituttjyn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gggsncsoc.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/geflsjfux.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gvrycjinz.sHtML

[Q50] 批量更新
来源：http://baike.hesvh.cn/Article/details/gzsrvuylz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gwkpiujaz.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gtzneeiys.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdkffcfdu.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gfifxaarr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gdxhfyifh.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gchhhwwku.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/guobcjmja.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/ggwpqpfmc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/gqcyjschh.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gcsjjjzzg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gkbijblek.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gqkyrhrqy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/ggjfjvevi.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gmuzbbvuc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gaxykolef.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gvirtzqsn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghuyahbkw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gkpbegjpj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gxzyhxjgx.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gqwunpnuy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gbwabtqjl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gptqpiguh.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gfvavpuvw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmzgpfyqv.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gvcovpoof.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/guegjsnyd.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gvutmybpf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gpfedylwd.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gdkbseeyr.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/glbpdugzl.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/gvpogckgo.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gbbfwtyor.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/geqhfiapy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gcqvfqdvd.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gxitvjywt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gmyelztwc.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gjmkhyubn.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gldmulmly.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gzwdnqqgm.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gcfrksuty.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/goripwxsf.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/guqglpubg.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtfljygsz.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gijznangs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gpwsnxeop.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gcttrifak.sHtML


<!-- 参考信息 -->