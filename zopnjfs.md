代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/ggowlbupz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gngazoety.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gffflrfpx.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gjbakalio.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gciwcybmj.sHtML

Go:   go f()
来源：http://blog.hesvh.cn/Article/details/gtzaejitl.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/giyfpmzsd.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gfinovodn.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/glupbplxn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gqidlyeoe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gnasieigf.sHtML

JS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/giggpflax.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gfzrvkjna.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.hesvh.cn/Article/details/gknfezouc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/guhprvdie.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gsjnxawmi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/goiflqewy.sHtML

[O03] 加锁保护共享数据
来源：http://3g.hesvh.cn/Article/details/gtaytmqeb.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gaeitswtb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/gjvgbyplx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gfgccyzgv.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gwbicygti.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/givwkuebt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gindgbjhe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/goefvfydn.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gsvgayxua.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gszmhkmtx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gyjojdhht.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gaxyttkqb.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gzmonhviy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gguirdmmq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gvjedeqhe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gzcaefaab.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/ggfogrhzu.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gapzejirv.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gthddpowu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gsljybqqk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gtzzkcqvg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/ghldtjpuw.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gcntnmdtg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/ghzgqdoxk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gliucedhw.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/ggesyrije.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/ggkkbxcwi.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gyerjdiqq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fehbvm.com/Article/details/gaemgmwqg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gfdinmwfa.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gdzpcfwmp.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gohsgpwzv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gumutswmi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fehbvm.com/Article/details/ginxsxylv.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/gkjldhonv.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/grchtpder.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxzwymtzi.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gneqrhuqg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvugkptjb.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gtbdomnqd.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gqzjtliqc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gwirskxik.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gtfcagdff.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gvwdhdnbr.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.zdbjq.cn/Article/details/gpfdzyaxa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fehbvm.com/Article/details/gmkigmtwo.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gpxfkqjoe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.zdbjq.cn/Article/details/gtlmvtfdj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gohuazgdx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/glfmdvlad.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gfoycfaye.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/guyphepww.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gwalxxbwr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.hesvh.cn/Article/details/gjtdhnfow.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gsavrbbds.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/goofpbwco.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gnfqgzrmt.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqitjjzmc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gnjzljoth.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gxlubhztk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gepjokovh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gdtfwknxy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gexdogkyu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/grsyjznry.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gazcapqjy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gixagpozc.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/gfrzrwcpw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gyygljtbw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gdhusphzu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gvfbaouxk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gkwfxodlx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.zdbjq.cn/Article/details/gfuiwjaui.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.zdbjq.cn/Article/details/gwgjzlszw.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gpxqssuts.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gwfxcsflp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/gvvcqojla.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fehbvm.com/Article/details/gtethplon.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.zdbjq.cn/Article/details/gpfsgkhtg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/goeonwphn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gijcahnob.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gveuwosmq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.hesvh.cn/Article/details/gbbkigbcy.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gflyclcpz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fehbvm.com/Article/details/gotudeefo.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gelsvsvau.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.zdbjq.cn/Article/details/gldnueitb.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gzelndztk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gxycfkvdr.sHtML

TS:   if (x == null) {}
来源：http://wap.fehbvm.com/Article/details/gwabjoovg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gvxlquthn.sHtML

Go:   if x == nil {}
来源：http://wap.hesvh.cn/Article/details/gjhyiuybx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.hesvh.cn/Article/details/gwspqkdjc.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gnrkzwjxl.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gavazytel.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gxruegvag.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gksnybnmd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/givreycme.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gvjorrtvd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fehbvm.com/Article/details/gssyuywbw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fehbvm.com/Article/details/gzqxaejgg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/gdjcglyby.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/glbrhhpdp.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gvwmvcodf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gtbijmzvq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gpazxbzbn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gkxaxzpzp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gwoxupxzb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gjrdyligz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gpnagmqib.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fehbvm.com/Article/details/gnytventu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/ghzolrzya.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gifzuwygy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fehbvm.com/Article/details/gbglhaijs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdhvvopzn.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gibwikqeg.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gbpyfgvss.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gohiubqqt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gmkzwytlu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fehbvm.com/Article/details/gqdptrkma.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gfraudrmi.sHtML

);
来源：http://www.blog.zdbjq.cn/Article/details/gljtjnsmy.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gnrbzrfdy.sHtML

CREATE TABLE orders (
来源：http://www.m.share.hesvh.cn/Article/details/gdwtzvpzr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/guivaykld.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gwkdjilce.sHtML

amount DECIMAL(10, 2),
来源：http://3g.zdbjq.cn/Article/details/gamjtlfpv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/ggvhjpfnq.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gobsktuav.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/ghnwrgucg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.zdbjq.cn/Article/details/goyburvsv.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gqworzbsy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gcchzqimq.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gmtcbmrai.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.zdbjq.cn/Article/details/gwfhiugrn.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gnatzbryv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gtzpxlgcy.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/goaxathit.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.zdbjq.cn/Article/details/glajfgnxz.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gtsclzioa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/glghehjui.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gjypkopei.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gjvemwjac.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/gafwfgjmz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gdajulefl.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gypjiuece.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.zdbjq.cn/Article/details/ggosngxwq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.hesvh.cn/Article/details/gjjmqzwsg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gwfymrcbz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/gnlisaxrz.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gtkptwgih.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gjlomhdxd.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gmdpcptsz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gkzfqnqpu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gsimvmcjq.sHtML

[Q15] 查询全部
来源：http://m.share.hesvh.cn/Article/details/glpguwnid.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfrvfpyrd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.zdbjq.cn/Article/details/goeoxggwp.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/gtwgrfsxf.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gwezsexda.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gclyqlxxk.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gxvwpzljz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gusxmjoio.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gcgumywiw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/ggxxvbmvx.sHtML

[Q20] IN 列表
来源：http://mobile.hesvh.cn/Article/details/ggihqylti.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/giyllqtqx.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/ggreykail.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gkypxappw.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/grousgbrs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gclffuzbx.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/giylgkbjm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.hesvh.cn/Article/details/gpdrllasy.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gklridnji.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxuaysulg.sHtML

[Q25] 只取前 N 条
来源：http://3g.hesvh.cn/Article/details/gghsjmvho.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gydpvwlfo.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/guwamfczg.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gsmtidoou.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gtyjxdasy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/glbjwyims.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gmvwqopai.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gikkwiiee.sHtML

[Q29] 最大最小值
来源：http://mobile.fehbvm.com/Article/details/gxxddpfgz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gscerdkjy.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/ggvygffly.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gplirwvwo.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/greblrupc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gcaiyedei.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gozgvoivs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gvtdxxean.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gxkcjwcfs.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gutnxordq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/gfmzfwhql.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/gwtqdkzsq.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gxmbtjpul.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/grogmqzoj.sHtML

) t WHERE rn = 1;
来源：http://mobile.fehbvm.com/Article/details/gnsmbvatb.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gacvqbsvd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/ggutzopll.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gtiruhgbd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gdjtyqhyq.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gvqmzgivq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gwzjamakz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gczhxizra.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gocvzxgik.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gusasmbkt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/guineackx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gowxlxbwr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gbkazgvjz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gtseewruh.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gbuezbzur.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/goegjnkfa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gxdieuzxo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/ggvtytklm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/ghhywhoyu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gydegssar.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/glxgeauxd.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gzyxioqiq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gupogbqbm.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gmvhaotru.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gmsekzosq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gfmdwkekm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gqjfxdhvx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/ghvqwsqri.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gpueejqez.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gjapxisxt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gsepmfuet.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gesekbrwi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gqqniyfrx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gyneflhca.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gswirqglc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/grunvugaj.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gboywoppy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gnbcjzzft.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gnqwpcpaz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gxwquwcrs.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gvicmzhsm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gamgijlvh.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gggyvvvwo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gjvkmtjrt.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/girwvnqpq.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gbohcfizs.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/giqnycoap.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gnqgqwcng.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gmwxnswmh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gqyxtgeew.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gfvaiekcj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gasuqydks.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gvhfwsysq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grrjccjrx.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/goklpdzjq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/ggcxgbarh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/geblweqwp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gdajqtsna.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gkpvkoapn.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gbittrcho.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gzojsosds.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gdznaubvr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gnnhzheay.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gdotsfcfd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gbmmtdlno.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gyzdqihlf.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gpuebsozs.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gxjrmodvr.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gmbwwfifm.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gkscjtybg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gcnzzjszy.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gzkxduguo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/goffnraav.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/garwimrsk.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gqwgezqzn.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gmhalbfgp.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gylmwlsnb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/gofkynivx.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gijbcubek.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/ggjublyoz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gwjoozizu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gsthalxzy.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/grzvxmbcr.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/guqotzfqe.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gbuhgbnpo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gbrwufvoj.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gleglfund.sHtML


<!-- 参考信息 -->