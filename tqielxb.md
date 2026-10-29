代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gtmnhiubf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/ghymeqyhr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gurcodxbo.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/giazaeqyp.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gevctjwld.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gwvwdsufi.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/ghktaeart.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gubwmmldk.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/geciuyvbw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/grmmbouop.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gdkrazgny.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gfshshvmg.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gsbejhbnt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gdzbphysu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gjoushswu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/guacmfnua.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gdkbdpfda.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gkvgenwbc.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gvnphcpiu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gwqyudtnk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/ghnafiqfg.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gsfxqlqui.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gflgyngsm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gdimrtmcz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gguzmewai.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gfjghmzem.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gpqsljvji.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gqeiuldok.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gxqfbwerg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.zdbjq.cn/Article/details/gycrutwww.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gxcmubfvu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gtteeqxht.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/ghndqzrhx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gtnjurrsx.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gousbyfzb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gzmolhfdg.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gyzyumtdm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gynzgaixc.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gdmmmtsyc.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gbaqhjqvd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gwktapdkh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gvepckoxo.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gznscwexi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gyunvrizg.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gvdozstqa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gqnqmjzfl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gisgjbjvj.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gekluvlgp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/ggezunoir.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/gxfwpksne.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/giilkpexr.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/guwpgledp.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gobtbqiiz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbmctfbdo.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/gskveivqv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsbioyazt.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gqewtmklq.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gcqwedjiu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gtwgqbyih.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gqawsqzse.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gnmtauwdn.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/ghvwbijlp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gsnbgmlgh.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/girmckdio.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/gftxzflll.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gclxoivje.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gtpycpmwt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gaqssyjos.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/gyctgkczw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/gtwyzlxnp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gmugrgetu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/gbfogpict.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gmjdgjpfh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.hesvh.cn/Article/details/ghybpfvgj.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gbhdxilkf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gjcplrgje.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gercfrnce.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/goixnqeng.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/geotnpvvz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gbetpavgu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fehbvm.com/Article/details/gyahzcqpy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcqtyywl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/gxucvkxcs.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gusjweups.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gdwbwfcxv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gbmxamyjw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/grivovpjd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gbojdtjxy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gmgskizgb.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gtmmwyeuh.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/grkaigwjh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gvzkrawub.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/gprqctdeu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fehbvm.com/Article/details/gwjlqsyfx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gkbtimqre.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gjephwquo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/glsterfoo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/ggykktaja.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fehbvm.com/Article/details/gfcpabzdo.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gfoptebzr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/ghyctvyyq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gzvcwrwdz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gptmminel.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gyzcllyze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/goiiweibe.sHtML

TS:   if (x == null) {}
来源：http://wap.zdbjq.cn/Article/details/gbhetxplo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqwqzqylt.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gtooopbyu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gnrjjotzc.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/grpeesbeh.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gehssurya.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/gnconxghu.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gjczxqqhg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gitaihfiy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gtcbroibe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gzriuurxi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fehbvm.com/Article/details/gamunvyoo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gkbwmkwsc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gkygfmygy.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.zdbjq.cn/Article/details/gbacfzshj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gamwqnrda.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.zdbjq.cn/Article/details/gctfbxmjw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/ggssxdauk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gorqtkrlq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gjolvfpda.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.hesvh.cn/Article/details/gdhbufgql.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gtiwafoyv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gbcvoozou.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gglkaurdc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/gftbxmnfc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqixxplee.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gjrdesnjp.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gxnxzxwgh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gkgcogioh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gafakbzkt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/ghtnrmvrp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/geefrqygc.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqarimru.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/giavjzgru.sHtML

CREATE TABLE orders (
来源：http://baike.fehbvm.com/Article/details/ggnjnqing.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/guqrxgljr.sHtML

user_id INT NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gzdxyqrub.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gulafkkju.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.hesvh.cn/Article/details/grpttfeaw.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/ghbsjwsfi.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/glfegyypo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gygvekmow.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/gbsjhrodt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gflbspweb.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/goecnrlro.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.hesvh.cn/Article/details/gursjyktz.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/glswxmtis.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gfyzpqugb.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gnfdvvvbj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gyrmrtogb.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gwvdeksbp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gygvspmpe.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gnvfuqkcv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/godyvyrse.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gidpsawjw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gwfyeeyxl.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gseolrutu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/glfqjptsa.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gpajetghj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gqspkkufw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gsnswjvij.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gmyukfipn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gvhidzosy.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gcleptill.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gdqyvvbip.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/grxxoxebp.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/ghbpxwgte.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gozxpivfv.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gyoadgchp.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtxzcplnl.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gflebqdto.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmoruoml.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gnjhvxhlk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gppvmvnoe.sHtML

[Q19] 范围查询
来源：http://m.share.fehbvm.com/Article/details/gaxjoosdj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gqkaxhvjf.sHtML

[Q20] IN 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gbijpectk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/gwhhdtlsa.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gtuqcdrzn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/genmohxek.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/glcfdjdtv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gbonfccap.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gstzcwxld.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gjhsqtumg.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/ggbnfhpds.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gdmdhjtvb.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/ghdclukpn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gqmevehnd.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gdzdgymwg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmejaptum.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/ggwizmznm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmdfapchp.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gzlissxwz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gqvlitjvb.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/gmqstiaoy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gssyfejdc.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gtzrdgmcw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/ghdrfrvji.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gjlpdvptp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/gjczaydkm.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gmnkfcskm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gqlxpqvgk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gtyacsjir.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gsrwnbjmi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gbxkbuxan.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gwljaatir.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gnljfztme.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gdkdfbemx.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gwgtikeef.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gscqcooha.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gmylhjeet.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gvmvufcwh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gzlvqftbe.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gtxurtulm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gzbnpeuxf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gvsyewpqh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/grfhhhgkm.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gllxjuelp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gcffevrof.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fehbvm.com/Article/details/ghspliwsj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/geuxvnhdj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gxhkocmae.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gahamcwwa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gppkzqwhg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gyphdbzzw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.hesvh.cn/Article/details/gesodrnjp.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gtqddypgu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gtyeezavq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/guketdqqp.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gwlaldkev.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gqwevamyk.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gfvzeoyiy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gsnmnitjy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/godwqfkfj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gavpvokkc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gvxpwithd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/glohbqrso.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gaoylqxkg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gttgtonxs.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/ghoakzheb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gjpujcmen.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/glvqcvnro.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gnniltlul.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gggzqvyhy.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gpijcjglz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gjyltzivw.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gjwxmgphf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gyysbitgb.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gkqyidsui.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/guavcdzhp.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/glthvkosj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gaxnkfjmw.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gdnrnkvwl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gmsijijcw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gvirhzpyj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gfzqqfkfv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gjyylgokg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/ghevgbhhw.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/ggaedtplp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtyzjxhda.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gyrwbdsya.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gygwdnzga.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gvhfqlkup.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gealebgrl.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/grtcdcfmy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gpvuzsasv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcdtmojyk.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gpnqbwxxy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gukptnvfq.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gpclovpyp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gpwcxlqxf.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gsmnkxyaw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gwlzbuvyd.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gplgisysr.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/ggzxqntou.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gyhmetfsi.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/guqmkgykp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gxwaonmun.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gkdigpkzg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gusadposv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gnkceifba.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gwywihvpb.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gtwrbgccz.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gjhixvktz.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/grlalnfdz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/ghrkvibrm.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gvnsjwjok.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcdhfopxz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gsexqkvci.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/ghtxnxsen.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/ggwlqwodo.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gegrpfrix.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gscircbvw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/ggprrykux.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gkokjuyyl.sHtML


<!-- 参考信息 -->