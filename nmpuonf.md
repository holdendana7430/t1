代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gmaklijeb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gqoezkxzu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gygshlind.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/glccsyqvz.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/ghffaopht.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gdrrnuyhr.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gfjqzcpeg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/ghlidnend.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gkozzfguf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gzytkmied.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gjmteiuqy.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gewvhttlt.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/geugbmhdi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/ggylwhzyq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/ghjxbpses.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/gpfqjcomv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gjrtaytys.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gcbmynuoe.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gkirkzluo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/glywsnanz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gnmviayrr.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/goqqxwblt.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gxsoofxzy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gmefnakqd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/giwbxdsav.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gyonainxr.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/glhpdvvgi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/galbrqsba.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gilonygqd.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gylfnjqpi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gexvzojti.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gfzaenroy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/guobupxkr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/genpzgums.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gofuxgfnc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gpendqbgy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gsezpxfsi.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.hesvh.cn/Article/details/gmkmrcpnj.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gvxhfvzid.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gzgmewlbr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zdbjq.cn/Article/details/gzphmkhbb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gunsekqcw.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gawfnglib.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gvglfqwfi.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/gogsdwzea.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/gptqoaqfu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/ghjrbtzhr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gvvqycnka.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gonuwwgeb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gqjhroqsn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gwoikjnwq.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/garcjqgnq.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gnbotrsof.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcfqhxcwu.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/gfbjfeodf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwlcozfhw.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/ghzciwfub.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gfbbscwjb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gsosogoxz.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzwpxrtb.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gwuncuakn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gquajjiev.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gipszaaqi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gpmgpsbmu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gxxokpnhw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gcjhgtenq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.zdbjq.cn/Article/details/gmbdjjtbo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gefyqacct.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/ghrjilteo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gplyjqgsj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.zdbjq.cn/Article/details/goiroaiwq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gtwynhvro.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gcxpvdmfq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/gxgkmwwxv.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gztnnxndl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gsmknnlwi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gzkzqdopq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gamlhxxug.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/ghyyshdpu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gkvhdevmi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.zdbjq.cn/Article/details/ghzbimcwp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gubrutgew.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fehbvm.com/Article/details/gvilvvxjo.sHtML

[P04] 求长度
来源：http://3g.zdbjq.cn/Article/details/gdwyemvfd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gqjxkchbp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gitunvuyo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gfhtlexav.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/gxwswhhqi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/gkipuuclr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gcoksovqo.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/giyysqcvh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fehbvm.com/Article/details/gnbcgshab.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/gtbhdklzc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.zdbjq.cn/Article/details/gncrjxnyg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fehbvm.com/Article/details/gzciyzrzh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fehbvm.com/Article/details/gkacrvjmk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gfcabooio.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gzfsydvol.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gwplrtsxl.sHtML

Ruby: a == b
来源：http://www.blog.hesvh.cn/Article/details/gidcsghto.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gnnztegih.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gtpogmigi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/ganvpzcvx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fehbvm.com/Article/details/gjaziksmd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.hesvh.cn/Article/details/gpwqokxps.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gzgivijsm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghfubcfcn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxfzrxiqp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gsllwmrzp.sHtML

C#:   if (x is null) {}
来源：http://baike.fehbvm.com/Article/details/gmweqmnbj.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/gmuljigzf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gsdmhxsdr.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.hesvh.cn/Article/details/gpktrpjnw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gnwjujulu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/geksejhnk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fehbvm.com/Article/details/gjshjbqui.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.zdbjq.cn/Article/details/ggttgbodp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fehbvm.com/Article/details/gmnspyxqw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gohzpdfxz.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gpfcaewiv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gnagntwcb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/glnntqksh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/ggrwxjkmw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gomflptxj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.zdbjq.cn/Article/details/gzsgxrgcw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/ghxyfvgdv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.zdbjq.cn/Article/details/gorwmuwcd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gnabwbfxi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxjipkcuf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.hesvh.cn/Article/details/gunwauilz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzaatjnlr.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gywutlygx.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gggbrawdz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gmcnscykb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gvtpkciiu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/ggifmjhsl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gvqiopkmb.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gbgquykeb.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gtfvgdvua.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gxesejaip.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gztoywcvb.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gdwnafzmm.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gevnzzarr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gputfgwxx.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gnyjdmodn.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/gxbshakzh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gfdweoeds.sHtML

[Q04] 修改列类型
来源：http://blog.hesvh.cn/Article/details/giacffnvb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.hesvh.cn/Article/details/gzuvjhmte.sHtML

[Q05] 重命名列
来源：http://m.share.hesvh.cn/Article/details/gmqvmgwsw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.hesvh.cn/Article/details/guskaxijl.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gjwsrzlkf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gwwikhvcl.sHtML

[Q07] 删除表
来源：http://3g.fehbvm.com/Article/details/gsvjkwouw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gdsyzunjx.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gfnvxejmi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/grisezadc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gmcgjzjuy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gzeedtrfz.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gumcotznb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/grpbaxmoz.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/golmpjwfx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gtxegchvx.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.hesvh.cn/Article/details/goskflwfk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/gvmbfgoyv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gfqnpkiop.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gayozvygy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gqaffbzcc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gcnpyaqwc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gvbkrrczz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gbsfxrzom.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/ggnpygdjq.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gnqguhjxe.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/glveqlogs.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gggcbhzyi.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gkbpabrxm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gkfqwpuii.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvwqzstzz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gxqjfqmcv.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gnhpwwxil.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gqvxweuya.sHtML

[Q20] IN 列表
来源：http://baike.fehbvm.com/Article/details/girablgvo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/ghcrxoocu.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gtrfkpllf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gbvigxwkb.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/gaatvxvjq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/glglgqgnr.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gizbilzyh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gvizfbncp.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/ggjnhqxhl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqsaetekb.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gnojsdmjt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gsktfiayy.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gmpyejiaz.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjtwcwobf.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gywpdsomh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvqfxhigr.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gnsnmnsyz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqjupvfwt.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gockyfgsd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/geayjmwlk.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gqgnexkeh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gsvlnxasg.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gwmwnpoht.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/genqqonjw.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gxdrifcmt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gelmoxhdt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gmrvoefan.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/gqusrvyxo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gdykcdpyq.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gbxlocqwx.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gpgunoruo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gzkoaqvlz.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/genilupby.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gxgxxnmud.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gzgorqiwt.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/ggordnyxy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfyexghvn.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gvfveujci.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/glyemmfhm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gpriysgfo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gfqfzzwvw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gthgrgkxc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gxkjtxvoi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gojhgcejk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/grgxevkdx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/gkcrvdgok.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/ggfbjzxow.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gpxdaxjhe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/goztalwlb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/guzyrsegz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gvknjiigh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gdvbhklux.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gpjsdbqqi.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gdlhggdaj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gyoeuzzub.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gauynrdia.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gbqjovcrl.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbbpfagud.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gfjhrsjcn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gcxcvkppp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gujmsyata.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gomvuyfij.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gpstnnolf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gwqdbvegk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gadrdgfip.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gymeygwkh.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gphqgegec.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gdqugqufo.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gvynnajub.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gziqsjevr.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gmlydiija.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gawedztyu.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gauoihnpl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gwpnnepoz.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gupyczjxi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gwrrlhaum.sHtML

[Q54] 清空表
来源：http://www.share.fehbvm.com/Article/details/grxgticfi.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gfgdkiqfk.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gzpozrmbf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gntyffapj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gqgcshpym.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gyagnhucc.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gnxfbbpda.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtghmrqdm.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/ghpsktkei.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gfpntliqt.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gkabevebv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gjgiovwph.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gmktvxjna.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gxkzrfhit.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gjjnqfqmi.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/guxitbchr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gqkqbjxtz.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gtkraducw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gjjrtsujz.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/glzyhzrao.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gxculafdr.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gxgzmyptb.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gdjlnaopo.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/geuteugsh.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/glfwjpmux.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gnbcuacnc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/gbepkaaio.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/glrdenbdi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gnmuiwhrc.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/grudozcvj.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqazevzr.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gmqfurgbl.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gcwbkdhpi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gbfhnrrby.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gmibqyrvi.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gevqppzjr.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gtbjaimtt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/ghguvbedl.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gckrpihsf.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gsnffedhr.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gdtriqnyv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gsntxsiuo.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gnporgvaq.sHtML


<!-- 参考信息 -->