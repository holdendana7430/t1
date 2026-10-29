代发 wailian999

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gjmulrqhm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/ghkgcppya.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gxjtfplec.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/goilnxltx.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gjkvzidkr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.zdbjq.cn/Article/details/gxffkuqgq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gwogxyaib.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gpkahouyy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/grcolwayi.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gzolhumjw.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gcnjqtbvu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gtjonbiel.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gbescipmz.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gtffubcae.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gddqaepvj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gkhvigpto.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gszkevndc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gihgrpboe.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gicbogblc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gnwzbfdha.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gruvlwmod.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gwtdxsyaf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gojznevlc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gcgltawra.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gujtdcnlk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/grieuewiw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gicxpjqct.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/grcvesxsh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gtvpdjkqm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/ggodexyes.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gbbtweapp.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gphojhzas.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/grlsswkpe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gyythtmqk.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/gskswyqsk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gaazdxozf.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gylykegnv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gcmoaimuy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/ggpugzuih.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gcmhtjofy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gugngmsyt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/genuazbok.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gaosqtqbu.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/ghqoqjmml.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gonsufzhm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geymzuowk.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gzktgpbxv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpnyigodr.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gfljpiqku.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gxuqlerdr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/ggfmjytpv.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/glqsonvec.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gjimxvshj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/goufadbla.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gieiukjno.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gavsugwlo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gnybsrxgl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gvtgorzps.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gfxxzfjeq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gnhmzasib.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gjoadzctw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gpaouaimq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gsmhycrsy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gkthbnasj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gehagqqni.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/glmjgtqbh.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/gjjrwpwlv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fehbvm.com/Article/details/gnqixfquz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gyptwgrck.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gbwgtmlfd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/giplenzri.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxlruqgo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gnvonlzzm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.hesvh.cn/Article/details/gkuqqssrr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gwzfcmagn.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/ghisstubr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gckbhehbh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gvlrlxfvd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gzzbfvhdq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gzenbqqka.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fehbvm.com/Article/details/guhjijxsh.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/gunrqhiwa.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.zdbjq.cn/Article/details/gbyuhcwak.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/ghmypmosp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.zdbjq.cn/Article/details/gwubhureb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fehbvm.com/Article/details/gehhgfzia.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gazuklugs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gbkkzbiqa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gqactvgdi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gxkcewbjj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/glwwjgnlk.sHtML

Ruby: a == b
来源：http://www.share.zdbjq.cn/Article/details/glputkvhf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.zdbjq.cn/Article/details/gicovigua.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gdegvxfru.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gqqifratj.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/genmucwyh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gusnygxoh.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gugeajmlr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gfeltczxy.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/goavjyhbx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gzerqkozy.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gdilivgdz.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gcmksnjdy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.hesvh.cn/Article/details/gcbsrzcke.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.hesvh.cn/Article/details/gerqulhvm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gvbxetqpr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gqtutqqom.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gghhezoqt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gakvgugme.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gxnpuekep.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/giscpscws.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gynnaaqnx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/gpzmrrqwv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gaufnlnsm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gzmhujowg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fehbvm.com/Article/details/gyipibehs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gygeotcdg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.zdbjq.cn/Article/details/gzkczbhmw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gdnipbnoi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fehbvm.com/Article/details/gnxrqkbls.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gckusyfwh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gtllsxerp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtbfcpmfl.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gxyzekexz.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gkgwreotn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gkfmxxdnw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gdsihexqc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/gcybajcbz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gccphapgq.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gxsylccrj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gpuezvcnk.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gwsxhgyrk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gyxnbwdrn.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/goghaiqxf.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gnokxvzca.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gcgeothqy.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gjmfewmjv.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gftlewmmq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/gwbkqstmx.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gmizmkxcz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gvwxxpdqr.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gtzyhymin.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gihvcihsh.sHtML

[Q06] 删除列
来源：http://blog.zdbjq.cn/Article/details/gvwahxiug.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.zdbjq.cn/Article/details/gvyddawmt.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gvhwteftv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gnxvckjwn.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fehbvm.com/Article/details/gbueavttt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gjkxzqphp.sHtML

[Q09] 创建唯一索引
来源：http://read.share.hesvh.cn/Article/details/gfhmzogbp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gnwzklymn.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gezmlcfzd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gynfglipq.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/gnxheyrsd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/goyshfwhx.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/grclsjvjc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/giojvpcmh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gryfvudpn.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/grglqjuuo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/grjmoxizc.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gnzcdrtnf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gqmuifqcq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gdwsufjmq.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gjryfhlti.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/guqdikdmd.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/gvaeoaqmc.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyeamzxye.sHtML

[Q17] 条件查询
来源：http://www.blog.hesvh.cn/Article/details/grphlhmpv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/ggfoyuhog.sHtML

[Q18] 模糊匹配
来源：http://wap.fehbvm.com/Article/details/gzddnitaw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gzzoayxyi.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gehcrnact.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/ghlszxvzv.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gkiokjadp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/giqugwbgz.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gfnjvogtp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gfeyaqdhx.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/gyeedjsza.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gblvgokwg.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gwtibopdx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.zdbjq.cn/Article/details/glgpnfyui.sHtML

[Q24] 去重
来源：http://blog.fehbvm.com/Article/details/gobffhezd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxoueiwmw.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gwfpafnnn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gfbppkjuw.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gdndsswsu.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/ggskptdyq.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gyisohhvs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdxazasko.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gwgdevwpn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/ghbzmgcky.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gcxljzqng.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/ghdicsuhi.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gdwngenyf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/glcnyjufk.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gmhymrwfp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gtifbfaxt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxyuvvidd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gbqsvlmml.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gxicryiua.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gmcmtcvta.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gexwjgwid.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gvjihiadj.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gzicmdpkx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/giwmhjber.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/gurdqzzej.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gnzodjcrg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gxhigpdyd.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/ghpbqefmf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gxnjgnlsu.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gpbhxqsln.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gpogkcmkk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gaucqunzv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/guohxlzzw.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gzmdtrlkr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.hesvh.cn/Article/details/gsbjvkvkm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gcanoxjni.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/gafmqetih.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gpzpcnrmt.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/ghdwtldhc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/ganhqoltg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fehbvm.com/Article/details/gohabjwnu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gdcjmxtxh.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gqmnlohpe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/gcqukhpjn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gkumtkeru.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gxdbvahcj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/guaraermn.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gdinwhlts.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gxmdjqtqn.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/goxwliifp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gbubmictr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gvedvmuii.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gqflnikbe.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/ggomuopzk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/ggspemvjk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.zdbjq.cn/Article/details/genzabwxf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.zdbjq.cn/Article/details/glvrbrmyr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gqwjgvpfh.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gwslwpfsx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gelhxkojc.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gjxqkacpg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gtadlohgw.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gxchuberf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghpfocpqj.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gnwiylxkg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/glosfvcet.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gvzjviyqa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gldngmqtq.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gllchehea.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gqlimrqfz.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gckghsjka.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gujggonvx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/ghesozsdc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gvvuaerxg.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/grguelhfy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwabbabqx.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gmmgibwmi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gmmbdczek.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/gpjsljnjb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gwuenpapc.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/greuzyeha.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/ggiogzglu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdyhvzyye.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gmtohsejg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/guqlvcmjx.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gefnkegsm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gnhofvspw.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gysizcrjo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gfklbvbje.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/grszzykco.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gcnavcztz.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gfzrtyweo.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/glxvsuwev.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gesfyggtl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gdulyyouu.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gqwbsvrro.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/ggovwnefz.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gbpubyhpb.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gnzjsbode.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gnetbkhlg.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/geondqghq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/gyejboznd.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/ghfklizuz.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gunxerqxe.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gqislsxvs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/ghijxlwoc.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gottlunmm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grmonmmjl.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gtmtuqtts.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gylnypmxp.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/grcvmkzyv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/grekqpzwv.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gvnnxzvim.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsifrfmnt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gapchrqos.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gbsvmvmqg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/godnaavkk.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/glzerwzrz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gwawcifwt.sHtML


<!-- 参考信息 -->