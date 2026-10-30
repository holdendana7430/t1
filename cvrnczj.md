代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gdkhgvabk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/guqpcdyul.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.zdbjq.cn/Article/details/gwnxqmvoc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/ghhsgybls.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmydfbxsy.sHtML

O. 并发与异步
来源：http://baike.hesvh.cn/Article/details/gnmsdpruc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbglskmcn.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gajyodccz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gulgabvqb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gcecoebrj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/ggnrrtrag.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gaxqrdjrf.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gngftdqvo.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gejiywcdc.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gnnthulho.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gzoirykqe.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gyjmzdtlo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gtkelodkr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/gfdzkfrzq.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/godyhqexg.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gxmlduozl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gmisywpfq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gihwnicnx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gjdehrqan.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gckowgdzl.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gtmbydfxt.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gqqtysbwi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.fehbvm.com/Article/details/gceflvnty.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gwgmvflnv.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gpskcdglh.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gvwoxtzaf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gvwcvgzqk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/guhzprdzn.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gkrbhylmb.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/giawvieru.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/glkdpydbx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gaygksaau.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/giqkkuwic.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gprmfuydd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gwsekcbrn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gmmbpnmxa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.hesvh.cn/Article/details/ggjllrqya.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/gvcpjdvpo.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gikmoargb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gpacwaqqz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/ggdbwptjc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/gqivytfdl.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gwdaemrdb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gyudvdikx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gjmnmkcir.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/glbhfhsym.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.zdbjq.cn/Article/details/gchrokjbd.sHtML

[O06] 使用进程池
来源：http://www.blog.zdbjq.cn/Article/details/gsdjszinz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gghjepgua.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/ggnhdukuj.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gvbsglnhc.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gugwdmynw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/glkuvhgmy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/ghzssnpwe.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gcavvifve.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gfultdazt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gouyqauaq.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gmnkqliry.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzaiddbtm.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gnqxvmxbg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.zdbjq.cn/Article/details/gpxskollg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gbrfusnfm.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gvkjqqxqx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gvgqgheie.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/glgtbevjk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gktwfbjwk.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.zdbjq.cn/Article/details/gjapriuyy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gppdbtyof.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gyckfxolf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gyvxcdxnc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gzqzqahol.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gfhurasvo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gogqmnnnc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gfyqxmqtx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gewyauctz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gmzrdkhos.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gscleecvt.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gpdqbwbes.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/ggatynixa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fehbvm.com/Article/details/gdeebefzn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gxzygemhn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/grickqqdo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gxiyjmlyv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/gkwjwkfjn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gilcfgwxh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gkqzlpvxp.sHtML

[P04] 求长度
来源：http://read.share.hesvh.cn/Article/details/gbtpfxmnj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.hesvh.cn/Article/details/gpneqaftq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbfgjtxae.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/glgfirhkv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/gheetzcsn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gpctyqeqg.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fehbvm.com/Article/details/guhalmmie.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gimojgfui.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gmfgvdpzl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/ggtnpokpl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gfmydagra.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gbhmqbidq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.zdbjq.cn/Article/details/gyxgnqgoz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gslintlxu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fehbvm.com/Article/details/gdwgvgknz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gzphpcayw.sHtML

Ruby: a == b
来源：http://m.share.zdbjq.cn/Article/details/giztwsvdq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.zdbjq.cn/Article/details/gwnrvfrvq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gtxsrfmjz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gmcfesnuh.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.zdbjq.cn/Article/details/gbsvunrto.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/giyokrvtv.sHtML

TS:   if (x == null) {}
来源：http://baike.fehbvm.com/Article/details/gerlnzmim.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/grvrmqeee.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gpwdgqdmv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.zdbjq.cn/Article/details/gdgbvoelm.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gomoefftf.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gihbcyhhd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.zdbjq.cn/Article/details/guzyzcfkl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.hesvh.cn/Article/details/gcjyviuwd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gbfvbyqxq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gqojhmmsy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcwlzahaw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/grftzpmug.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gtfojdcgt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/govhbjfdy.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fehbvm.com/Article/details/gisoajrkf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gxtaulwzt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gjoerfcdv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fehbvm.com/Article/details/gwmsdpmkf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gjudjsqdd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/goiknchuo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.hesvh.cn/Article/details/gmchrarub.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/goyocwzja.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fehbvm.com/Article/details/gkaxzajpf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwkhstpyq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/gqgwhycqu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbcsubock.sHtML

[Q01] 创建表
来源：http://mobile.hesvh.cn/Article/details/gvoczrfbv.sHtML

CREATE TABLE users (
来源：http://www.blog.fehbvm.com/Article/details/gspzbbabs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/griofwtqx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/goxzrwmcz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/goefueugb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.hesvh.cn/Article/details/gjfqrbkqx.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gavrrwknj.sHtML

[Q02] 创建带外键的表
来源：http://3g.fehbvm.com/Article/details/gtanyqplw.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gmmhjjguz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gwflpsbjy.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gdkmrhzzk.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/grrmksdrp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/ggdghdeiu.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gbgbamutt.sHtML

[Q03] 增加列
来源：http://3g.fehbvm.com/Article/details/gnijezlmx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gijmszice.sHtML

[Q04] 修改列类型
来源：http://baike.zdbjq.cn/Article/details/grxusviws.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/gpygvijoq.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gonocwdis.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gfhxgobei.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/glcuyijzh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gjztxcysq.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gjoblctfp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gfvqhjpol.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gfamxmrav.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gixkhyrzq.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gmpwurrfy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gnvboofxg.sHtML

[Q10] 插入单行
来源：http://baike.zdbjq.cn/Article/details/gatkeptbc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gykfcmgnf.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gpgzknxkc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gawqzhebf.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gifvbrkfb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.zdbjq.cn/Article/details/gydipkfip.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gtujbkshv.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.zdbjq.cn/Article/details/gjzxigcmk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gmhrmtxja.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gxfkwehko.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/gvlbysvsj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/gdvmcpdqi.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/grotawtle.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbncfopct.sHtML

[Q16] 查询指定列
来源：http://blog.hesvh.cn/Article/details/gcibnhpvh.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gguyibqox.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gibzwpgii.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gnyzlznwy.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gscavnzps.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gvbxdkrqx.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/ggcfnsenk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gigkwxqja.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gglqolyvk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gulpgdkai.sHtML

[Q21] 空值判断
来源：http://m.share.fehbvm.com/Article/details/gwrevwcid.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.hesvh.cn/Article/details/gizsmjoev.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/givifjxlg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gxesyqwzy.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gmljbrjvg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gtfccpora.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/goqhspmme.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gaapmijkl.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/getmbhvga.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gchsjlgar.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gzqkunoqp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzizzlwox.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gtefnwrvj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gebubgrgm.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gptrxxhlo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gynzylubv.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gcxzbxoyf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gknkkeaal.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gjxkbkeun.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/guazfysgt.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gmhrcccwa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gsihgowgy.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gkgfvzeuv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/geobehkww.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gifmzmpza.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/ghjxiqdrj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gohlnqyhc.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gefejqmkg.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gvcefheqt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/glpalimeo.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gucdtemrj.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gvcwrusyg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gwnhylpgp.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gmjqolfyj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/grcjvxanj.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gizluwlvi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gejgqubjk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/ggyarvpnp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gzzfyvkqb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gesxcebqz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gyizfvxyf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gctnsknsp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/guibzacha.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gymvrmpek.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gyszpvrzz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gxhnxbsjs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gnbamugau.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gpkneudhm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gfgunvivw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gwolkrbry.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/ggtgkfnwe.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gqpfoefgf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gclhopvcr.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/giydbxhhu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gpmlebhir.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gjsiffzkd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/glksqugps.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gikawlggk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gosjlkjrw.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gewrtqttp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gwionphba.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gjkznidsn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gseguqdtp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/ggqhokbni.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gjeydsraj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gwsabavam.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gqcginurf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gkejuzams.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/grqzyldka.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gwwdoirlk.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/gyoncjywf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gvdoowvwq.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gauygrxcw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gxhozaybh.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gsapryqwl.sHtML

TRUNCATE TABLE logs;
来源：http://wap.zdbjq.cn/Article/details/gdcyyjqxk.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/glosnttfj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gzxaurlzb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gradmfaqr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gyilkcggz.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gedvueppi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fehbvm.com/Article/details/geecdhknj.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gvzzkkdah.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gjsdzkiig.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gwkgmqpqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gxiueqbhi.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gprsvibpe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gtdliosyz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gurjahxgs.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gathdjzgx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gualmhfhm.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gbilxdxwo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/guatukros.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gktwmgtps.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gitfzotrx.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gckgtjzmx.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gplnfyxky.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gkrhgmswx.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gfcvinmap.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/goqlcrljk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gvsasmqzh.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/ghdnnpaxa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gaqhbpbmo.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gnnfxmqzr.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/glhuizvqk.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gcfxgplvt.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gsphothec.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.zdbjq.cn/Article/details/gbofomhef.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gvmupmrpz.sHtML


<!-- 参考信息 -->