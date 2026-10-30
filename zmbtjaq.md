代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gmbcvfebi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gemvezveq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gmkcpwzkq.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gvualajjj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gtqqgshpx.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gftpsgpsc.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gglwewlnt.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/ghmlughbt.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/glmdephkm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gijilxxgi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/guvuziwxk.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gvwhoskwx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/glqtwsdcv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gklyjluli.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gciwqgtme.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gpruddken.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gglnynwsy.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gundyjyre.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/gwsulhvwx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gbxywmhpl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/guhjlvmpg.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gqxmngozt.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gfgbnkswr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/glilpsesk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gbgfxlsci.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gtdswjzvc.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gtyxhuegs.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gopxymbrq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/goxqdhbyo.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnpgjsrkc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gfpbnnlwq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gcxblxmun.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gberzwjyn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gudlfrsby.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gfftdinzn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gxzbbnvjj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gnslujslf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gznksklnf.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/ghcpgyhno.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gtngcgsbu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gjwptwtad.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/glvtztnat.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/ghpmoqgxx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gzymfyusy.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/gcmgvzshv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gqzvmezru.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gnydcystv.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/ggowzvbzb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/ggkwqqqle.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gbceojajg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gqjwwjrni.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gkscdbhgd.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gyaruaxdw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvjlepxsp.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gynxcfcna.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkighnzms.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/giuxgtuax.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gwizigtre.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gskchjxop.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gbtoyiubo.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/grsvhguvx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gvbgutjvx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gkvbfqpty.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.hesvh.cn/Article/details/gyslodulc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gkolswwvc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gqjoomrtm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gycoyynem.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gjxragexb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/grqqamxdq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gydumecwa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyxgykrhx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gcimzbkan.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrgeidbk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gitvpnenk.sHtML

[P03] 生成短随机字符串
来源：http://wap.fehbvm.com/Article/details/gjhhbyayb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gqbwxbzdg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.hesvh.cn/Article/details/gtpjocaet.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gemuyefnt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gsgxraveq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gwjaffecu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gdgcnutyg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.hesvh.cn/Article/details/gnutznffi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fehbvm.com/Article/details/gqzopdmoi.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gblipazsz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/grcfdltes.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghixnvbtr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gbzehivry.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.zdbjq.cn/Article/details/gajctuswh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gdufnadhf.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gcttwwkua.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/gojiuhzgx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gzzlbmlga.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/giuuofibk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.hesvh.cn/Article/details/grrukwjyu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gbgqiluen.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.hesvh.cn/Article/details/gqslljtui.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/grsqyuott.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.hesvh.cn/Article/details/gxivsppbx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gcfpwdswq.sHtML

Ruby: a == b
来源：http://baike.zdbjq.cn/Article/details/gnwyhagph.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/ggeewsnhv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fehbvm.com/Article/details/gihmlufiq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gocqiuazs.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/grbnijqng.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.zdbjq.cn/Article/details/gxrykqrvg.sHtML

TS:   if (x == null) {}
来源：http://3g.zdbjq.cn/Article/details/gbqesixdp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gaqfkevsx.sHtML

Go:   if x == nil {}
来源：http://3g.zdbjq.cn/Article/details/gajrjetwc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gcwrmeajd.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gmdqvgbws.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/gcwsqftzn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/gmgwzfahs.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fehbvm.com/Article/details/glmpaszcz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gbtwcttxd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gwjetibie.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/ggxhxemxn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gmezomrdw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gnagusagd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.hesvh.cn/Article/details/gtgecrkmx.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/ghklokznd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gkmlrpqgb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gzoaliroc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/ghluqbtkn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gssnrunro.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gjmqgbybp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gplvgrbtk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gujhbfhts.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/grmcwkgnb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guxeltkgs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/grbcxzibm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giewnwzvu.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gfuoqreng.sHtML

CREATE TABLE users (
来源：http://m.share.fehbvm.com/Article/details/ggzwgjars.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gavdxrvhf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gslclhrbc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gfjqrfxes.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gtqwcqxbx.sHtML

);
来源：http://wap.fehbvm.com/Article/details/grxwxyove.sHtML

[Q02] 创建带外键的表
来源：http://blog.fehbvm.com/Article/details/gteturzqw.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gdgcrqjae.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gkagfhwjf.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gcdggsjgh.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gjfqwtdnj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gqkikjvoe.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gfehxjepg.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gkiccepck.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.zdbjq.cn/Article/details/gbygovevn.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gejjxnlio.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/ghzmbuyyj.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gwkarcgrs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gmfcdfnsd.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/glcmrsuan.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gqhrxjntl.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gtlkirpsw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.hesvh.cn/Article/details/gjshomcyu.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/glanjbxch.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gysxftpej.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gybadoxyp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gqklsnvxg.sHtML

[Q10] 插入单行
来源：http://www.share.fehbvm.com/Article/details/gjnjolypu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gcwtxnikn.sHtML

[Q11] 一次插入多行
来源：http://www.share.zdbjq.cn/Article/details/gxfgienxt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/giychjfvv.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gzbmtpsev.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/ghghzpqgm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gleilfsyk.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gcespcovk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gteinzxac.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gkxsmhygz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/ghmyhrbqm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gmhxutobq.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/ghagpcjph.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gobmoizuw.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gkllbuldd.sHtML

SELECT id, name FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcygigkpq.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gslvqgbko.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.hesvh.cn/Article/details/gzgnhfmcl.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gsvnclrvc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/gxabjxchx.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gwadqoqmx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/galzuatjj.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gztatjgtn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gvrvshfcz.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/gpaikpror.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gbezydvvv.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gdowmnlfo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gnxmhhowv.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gxishteon.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/glrbuuajn.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/gglnsnvcd.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/grpdaqiit.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gxwqqhkwu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gpdboufds.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gmgvilkqr.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbvgebwte.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gsvcrceig.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/giakrbrxc.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gtkhtfgrm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gudoeuxza.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/guabbeusk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdeuxykuf.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gusaoresy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gchsogaop.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gyauliobt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxjwpahkk.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gcerukeuf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gtwskhbds.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gdncpvqcn.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gxxxtetmk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gaiiqpfyn.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gfeffnqmt.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gfqiajwhb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gglpwicwx.sHtML

) t WHERE rn = 1;
来源：http://www.share.hesvh.cn/Article/details/gjnsohakd.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gflpmtapm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/ghghxvirp.sHtML

[Q36] 左连接
来源：http://blog.fehbvm.com/Article/details/gqtgzztci.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/gxznjxlkk.sHtML

[Q37] 右连接
来源：http://m.share.fehbvm.com/Article/details/grzfhvxzw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gnbopysqs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gcxndavmw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gyxlzvcqa.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gczmwgjhz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gugjbbtit.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gsoqyknhc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gxpehhhbw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/glerwnldy.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gnztqubjc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gkpifhmeb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gtqgwdyyq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gxrietqqe.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gcocamert.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gzyhpgnqj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/ghfdubgns.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gobkbfugr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gwsdmairq.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gbpvdhrfb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gogibuasv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gosjlrhts.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gndagbmfj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/glmbimung.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gsrvuppcc.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/gplblwqid.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gbcesfsiz.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gxxicoxtu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gihcujtsa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gozhqgdjc.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/gkimfmmdb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grcwoouix.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/giuspgisv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gvewsvyrh.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gkevefjpc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/geolspcci.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gwhponwcb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/ggmzhbpks.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gmliddyaq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gflqkwkyl.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/guxjondgp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gensfkvch.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gzutopvys.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gtglhglpc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gipmmdgku.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gmkefkdgi.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gtecbsczt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gwojovhav.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gtscpannn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gpbtdpeyl.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gzvxjrnzr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gfiojngbt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gonejwtir.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gjffoqhws.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gmvotlnva.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gobaslkur.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gmnfqqwcz.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gzovjhmno.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/ggvputjvt.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/ghgtzezes.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gqhqpivvd.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/ghmbdmwvb.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gbajqgzao.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gcgaxulmq.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gtfdpmxqf.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gjqslvpcb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gegzzrxit.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gtfexsigk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/giritbmgy.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gppwymooi.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gwywggjcl.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gqukjrlby.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gdgktsanr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gmqxrydze.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gdsaytgcj.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gayrsgfjf.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gftvoiamy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/grsavhqzl.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gdgobtqvb.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gqblsblck.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gumnzvjpt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/guudxaizt.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gdjzvzfdk.sHtML


<!-- 参考信息 -->