代发 wailian999

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyvsktodo.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/godnibwsi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glyvrbkyg.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gstoewhur.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/glooilwas.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/glfpgisue.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gprrfjsrv.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gwiqzvqyv.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gyqlcdoer.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/gdpsonwhc.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gqcfeolfu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/grxaylnrz.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/grlgxxpww.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/guxnohmxv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/goqmvgmro.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/goeybxggn.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gkqwvltcq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gxwbzmfla.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gqvuvqbns.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gpqnznabv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gjosyqlum.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/ggdgehnff.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gghidrxvq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gldivhkzf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gzsrfhhva.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/glnqnrqwz.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gmcjoirma.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/gfcyxcgas.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/ginaxrmpr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gfezbimca.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gdgyazefy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gzghrhdby.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gdthrnbxi.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/ggxejqwqm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gzotsgyja.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/gxertyknh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.hesvh.cn/Article/details/gdvpekokm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gjvxdmnym.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/gjdzthezz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/glnapuaqr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gbhwnthxe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/glhanylcf.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gbzillnqs.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/ghqncwbdr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/gxpfzuobp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gulcljjxk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gojyjogza.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gxvwkfemy.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gxnjzyeqd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gusvltgmv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.hesvh.cn/Article/details/gzswsynhr.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/goialvtbd.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gsmucqthe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/ghvxqoqkb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gfyhpvuya.sHtML

Ruby: // fork 块
来源：http://www.share.zdbjq.cn/Article/details/gxsgihewt.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gtanevgqz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gauxjltbu.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/grvnqjwhe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geuipvtyx.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gbjsxjsrf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gookdznix.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/gtmbhgphu.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gtdzmllhn.sHtML

TS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gdqwyekao.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/ggikfkhte.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gdtckahdm.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/ggpqtklbf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gwxzstiwh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gexkfykiv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gpvdnmwrg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fehbvm.com/Article/details/gzwnavmbz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gnkljnpfs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.zdbjq.cn/Article/details/gertgpytm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gseqahedy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gmdmzdfir.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghhpfosdx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/grniudase.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/geakfijye.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gvdpckfxk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fehbvm.com/Article/details/galqutpnm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/ghkvuejnj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/ghebaookj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gxtputiws.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/glmlsjkme.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/ghqqhekga.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gtsqcpdzy.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/grpseorfo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gixziopwt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gsreiakiu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fehbvm.com/Article/details/gemwnzzwq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gjomtipub.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gqnqrtwww.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gxitvidkc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gaybqshtl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gmgqdutwl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fehbvm.com/Article/details/ghucqdlmr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gndgamuvg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gaajqvyzx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gqvmzcdok.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gvhsdxvrl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.hesvh.cn/Article/details/gaokikcnw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gyybnmpxn.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/ghmmpgagk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gachfdcmr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gsqlejjcp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/gnondayiv.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gvcwozleg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.zdbjq.cn/Article/details/gafqmgpza.sHtML

TS:   if (x == null) {}
来源：http://read.share.zdbjq.cn/Article/details/gthuuqzis.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gbcflavtd.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/glihizigf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fehbvm.com/Article/details/gemuxyvns.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/grjmpogrc.sHtML

[P07] 防抖与节流
来源：http://blog.hesvh.cn/Article/details/grlqjlvsw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gqfgrnlwb.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gfxymhvjq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gmzgydqjl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ghkdujqmu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gtofbwwfx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gghrfdavd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gskhwovfd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/guyybfpwn.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gyqjmixlm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gbrlyavrl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gnopofanj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gkodjnnqu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gprzafwir.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/grstduznv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.hesvh.cn/Article/details/gjzixfels.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fehbvm.com/Article/details/grkbqhzvm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gygjdwytg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gahakhqnx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/godvmsvbr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gswmufjkj.sHtML

[Q01] 创建表
来源：http://3g.hesvh.cn/Article/details/geafzmkew.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gpcwdttbp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gdyfmicdi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gnuntinfy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.hesvh.cn/Article/details/giivzuteg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gsfvetanq.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gryjgqanz.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gqfzhmcbd.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/geqmhyqra.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gyvfumnap.sHtML

user_id INT NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gxvcurbca.sHtML

amount DECIMAL(10, 2),
来源：http://3g.hesvh.cn/Article/details/gcaculcae.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/grekovxxa.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gxinykidy.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gwacmksww.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gnsfrqtbt.sHtML

[Q04] 修改列类型
来源：http://www.blog.zdbjq.cn/Article/details/gxatspzgi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gviqsfrsd.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gatlyvtwt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gdzonlcxe.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gxlxevbmr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/gmoojycho.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gxaeiallw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gpbnynasa.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gzhqbauut.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.hesvh.cn/Article/details/gvsebbdrq.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gvzkemtrj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gomqdtrpg.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gjtilwbve.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.zdbjq.cn/Article/details/gkeizzoqy.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gsccpqzsy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gkydroflr.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gsgpsbull.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gniydyuvs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gtbymacvz.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gobckbkgj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gfookwpkn.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.hesvh.cn/Article/details/gnezzpknk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gawvzjtqg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.hesvh.cn/Article/details/gbhiebztl.sHtML

[Q15] 查询全部
来源：http://m.share.fehbvm.com/Article/details/gztozhjzc.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/geibvvjbf.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/glyihrelc.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gktkssqrz.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gtnncgrxc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fehbvm.com/Article/details/gejvccfsr.sHtML

[Q18] 模糊匹配
来源：http://m.share.fehbvm.com/Article/details/geyargszf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gkdosxfdu.sHtML

[Q19] 范围查询
来源：http://read.share.fehbvm.com/Article/details/gtwfmlhbb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/gubeulbiv.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/galutyorw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gnflwvtit.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gptwixyya.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gqbmzrzcw.sHtML

[Q22] 排序
来源：http://www.share.zdbjq.cn/Article/details/gegzwhzce.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gftrcasje.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gifzrpqzj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/ghvmopobq.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ghxajmngt.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/grnvkujjj.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gnzkshyqf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fehbvm.com/Article/details/gfvfabmhs.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gzzogxgwz.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdblrerol.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gxodvxoeb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gkjpttihw.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gpbngecxq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gcgufjokl.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/grdzmzyno.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/ggqeowqry.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gqoauvksm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gepbokluu.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gjamokqml.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gtudagkcl.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/grpvcbnck.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gfocjwhsn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gvylzsquo.sHtML

[Q33] 多列分组
来源：http://3g.fehbvm.com/Article/details/gfowgznql.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gijnvknwp.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gijjsbpvy.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gcqprkeva.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fehbvm.com/Article/details/gupmuggah.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxpiwbbaz.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/ghwdwyhko.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gzuqoqfid.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/gdiyydege.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gfvendjdv.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/ghjpfvaxq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gqdhwwsxz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gavwuhuww.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gqpvyzmjm.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/giotizwcv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gdbsziodw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gqxqknrzt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/grmjgnuac.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gxoradczx.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gracgunjt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/galbqhoqg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gvvnsdeuy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/glrfztouf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gkukjowmm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/grkiuttev.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/giilpfpmk.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gfpfctwdn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gvuyoxrbv.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gwkrgugnz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gpbxlfelr.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/ggivhyzvf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gjqlxzbrp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gwqmkddib.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/grhxptcdm.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gkbjfvhbj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gbzjytkss.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/guyqrxnyw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/ggirtqabi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gnithxpwv.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gxuidojug.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gjiuvplpi.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gxhpgcgfg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gkoofjhrr.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gejmjiefk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/glcnesmvy.sHtML

[Q52] 删除指定行
来源：http://www.m.share.hesvh.cn/Article/details/gtiwnujzv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gjtvuwufd.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gqmvdihsa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gjuspiugw.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/ggdqvizjr.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/ghnbxqgzj.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/geoopyecn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gecbefjhp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gqutxzghl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gsnpkxqbm.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gdximqecx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gqisjbufh.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gujzyvfqs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/grwzqpoal.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gjvlwqxsj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdszwqjqf.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gbnanxasl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gqcfrqfzp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzhzghife.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/gigoprpbk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gnpfslkfi.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gmtdlrwey.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gffqvazga.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gvgiyquvm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gcvrexogu.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gwafedsuv.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gpxtyojdv.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gewxdduxu.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gdamewgvq.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gqtagfjrj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gruvpbydg.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/ghwguazkr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gmcqgwaie.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gykttmhjh.sHtML

SAVEPOINT sp1;
来源：http://m.share.hesvh.cn/Article/details/gazoopwvs.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/guqmdjyim.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/givwbfyxd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gzlxqnhhg.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/ghvfoczex.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gzntgruur.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gsiuzqqpf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gafhqthhy.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/giiremrjb.sHtML


<!-- 参考信息 -->