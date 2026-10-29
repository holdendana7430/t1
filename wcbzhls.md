代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gdvxyscwm.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gporrchhn.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gqrrwtnji.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/ggmwelbpz.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gwrvgceep.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gqolkjqlm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gfqntbhef.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gbqxesefs.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/ggjglcjlz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gtnhlqdsh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/ggkittgmn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/gqtfgzloh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gudhrnjvh.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gussbkara.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gnobyrdzo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gtxakhcbs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gfffretxj.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gcicdaohj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gsjruhokw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gtdjiirdl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gcghetpll.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gylcufxuz.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gwhzulxex.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gdynchqti.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gkopcnicr.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/gfxdyenmx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyphtxpyp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gvuoubrlf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gznqhtgkw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/ganfnzauz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/ggkdvfrtt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gwybaziwy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gdxsswyln.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/gelzzgerb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gzicgjccw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gzmmdkrpi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/getlzidjo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/gahpyrsyl.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/gjjyalkrk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gjiryirav.sHtML

[O06] 使用进程池
来源：http://www.m.share.hesvh.cn/Article/details/gfujtzrou.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gxdnaadaw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/ggkaqgqvl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gcvghjpmn.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gpypegtub.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/ghlbtcgpd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gnieharqb.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/gyccjtysa.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gwwckqmmt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzwwdthyc.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/ggvjvwxyw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvzetithk.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gbzyxcxfp.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/griumvftu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gylubgmmj.sHtML

JS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gihowxcca.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gtpqrokup.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gmmfwrhvo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gfizxilni.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/guauzeiag.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.zdbjq.cn/Article/details/grafwwmhh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gwyaormyt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gnztvozjo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/goesgynnb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/godldswpf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gsmpehydr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gufmxxcda.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/gizvhmgra.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gmwhbjjnh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.hesvh.cn/Article/details/ghumduynq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gdawscart.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/ggxalrxjj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gzrojsaod.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gtecurwaf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gtngvkoll.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gbatmzrla.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.hesvh.cn/Article/details/gcxzxztdp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gypkmnven.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/ghqasdapx.sHtML

[P04] 求长度
来源：http://read.share.fehbvm.com/Article/details/gjcsamaxt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.zdbjq.cn/Article/details/gevydjpsq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gdnqsqyvv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/ghyonohke.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gkossrkyp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gcqtvfxpk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gtnppmghk.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/ghkgzlcdn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gaowranol.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/govoimwfy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fehbvm.com/Article/details/gtnylzdwc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gppiplztq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gwcmicivp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gwqkivcnf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gembsfspy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gevvjyczx.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gwvxuyipf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/getukrcgr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/ghibnceag.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gwzxzputv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/grljbnxpg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gpmzkjbvv.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gjwhonkfe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gzfgobyhx.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gwevaymbe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gowdsxtos.sHtML

C#:   if (x is null) {}
来源：http://www.blog.zdbjq.cn/Article/details/gktjtnfrn.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fehbvm.com/Article/details/gvkhrpidr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gptltdetm.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gdvccrene.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gmmmsyjqm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/goqomcmcr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fehbvm.com/Article/details/gokwktioo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gfiexllqo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gjxpqpiiw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gqbljcdgb.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gmvjueict.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gzsosvswr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/ghzyaowem.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gwatihvph.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gjmbpviyj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gonxtcfnr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gepipbnyz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.hesvh.cn/Article/details/gjnofgejd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/ggkhxeira.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzegauymg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gypirsbfi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grxrrqhvg.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/ggpuppjou.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gnqvgofdj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gyccjpckp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/grzefklvb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gvhvcmmna.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gboypslmt.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gktthzbjy.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gogmbdegi.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fehbvm.com/Article/details/gsmkdkqoi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/ghulnbdgg.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gsbeocbfm.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gouyiuzev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/ggytbqrqr.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gxskjwdcj.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gehemxvyf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/gmrsgwmlk.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gjvzboznz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fehbvm.com/Article/details/ghvlppmsx.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/graillfuj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gwekbouzx.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gbxkykggr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/godqookmp.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gezxahium.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/gviyojzag.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gncgnqtbj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/geuoxbmxh.sHtML

[Q09] 创建唯一索引
来源：http://3g.fehbvm.com/Article/details/gkxlmvgub.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/grfcfhdrr.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/ggypbfpzb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gkcnyadby.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gbytgtqzu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/goivplktk.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fehbvm.com/Article/details/glzlmcaen.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gcxjdjtsj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/grxodhoim.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gvopqkdez.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gmqegbwhs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/ghsfletek.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.zdbjq.cn/Article/details/gjhgphlnx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gptwqnctw.sHtML

[Q15] 查询全部
来源：http://3g.zdbjq.cn/Article/details/gnyzonpzm.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/geosplygk.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gnfaarkob.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gyfgnsjuw.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/ghgkboaxw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gcuwlhdhy.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/goefmpqlt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.hesvh.cn/Article/details/gdwwymdqz.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/gfkkorocz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.hesvh.cn/Article/details/gjctpjuya.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gldulwzaa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gfvwnbrmw.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/grptcchjy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gcuyngzth.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gpdsdvtpk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/glupjljay.sHtML

[Q23] 分页
来源：http://m.share.zdbjq.cn/Article/details/gjoirubmi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gmjaexkcy.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gzvtvnycy.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gihzyrufn.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gpwxdqicd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gdowqlyvt.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/grphdskgp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gsygbdchm.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gsjyvglnm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gzqahsrro.sHtML

[Q28] 求和与平均
来源：http://read.share.hesvh.cn/Article/details/giqdudrrr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwbjgxmha.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gdlvsghwa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqsibooza.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/ggegwlreh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/guogkhuws.sHtML

[Q31] 分组后过滤
来源：http://www.share.fehbvm.com/Article/details/gdirfmhyi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gkxdbifcq.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gtheoefxr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gibsqmpbm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gjjuvmbfe.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gqiwroodf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gygwgevlc.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gosoafrwp.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gawwyoknw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/ghsxngram.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gdksqrtin.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/glltoywcg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gwtmjpfsw.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gmwoivqhb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gkgbbnkkl.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gfhkppxwb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gewofnozf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gwdvsjjrz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gzrcswztn.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/ggqbugkfp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gzxkgmglf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gbuhuwcwd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gqwfyzlsz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gxgljxbjw.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gbpkgrtbg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/gmlpovssc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/grmurqtrl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gqnlksget.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gksjefzjg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gdaslrisi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gluuulfuv.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gwuqeefvk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gupzxytrm.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/glerdxtsj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gxnnlejzs.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/grtduoaer.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gmppcxppq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/ggdjfnijm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gtmzvowhg.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gsfxqmwau.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/goxbseqjv.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gpuqzthok.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gxemflysm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxripqm.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gulyrbymu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gakglwjgr.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gqlpqkffn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gfunzutgz.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gxsmghpir.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gswffsmuk.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/glcuxwlne.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gjjmsesoo.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/goiykjuvl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gaarwrfqy.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gknjnqqvj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/ggzdigzgm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gasufvssd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gljwzeexs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/grftqtqay.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gwwndffwt.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gsjgnzkvh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfvbmmior.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gzgyuzdis.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gqkilwwfw.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/grigfvhju.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/grenvbejk.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gnvdiowke.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gnpbsjvzw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjehqfqxw.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gdwxwgfpd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/guvsxvtsc.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gygocxrnv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gywitkxll.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gblhiovqq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gcygwptgg.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/giyizpjvc.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gjmcrcema.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/giuydcdao.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gbwiwzddw.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gvovynoko.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gxgskzqie.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gxrlapsgn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/gwwoyvdoe.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/gwywzigun.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/ghkdiitwd.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gbufedbqy.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gnmaxeuct.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gucyfqphg.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gltxxtroh.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gwardldyf.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gbnxvvflr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gsrcjexgb.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/grpfusaqk.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gygsmjduv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/glfagpsis.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gudmoxumx.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gszasnsag.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gqpetglfo.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gjtrcwiuc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gwsgmwinw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gsiotsxpv.sHtML


<!-- 参考信息 -->