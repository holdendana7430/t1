代发 wailian999

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzjjiqqia.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gxgckzran.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gothfcvcp.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gfosngzpp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/ghkdnfnsq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gmllvwdlq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gjscknsxp.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gjwbfcpti.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gfmxacjnt.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gzlfwqmge.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/ghhswserk.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gaxejwems.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gknhucyno.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/goyqzbres.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gopbtrkhx.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gjschznhg.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gdgzwhwaj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gtmzlbvez.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gzvhtikku.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gpwfsrxfq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gvwtnhsyo.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/ghgvvglgm.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gdnkowmab.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gfvhjqjge.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gyxnzlxvw.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gikyvlbvp.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gvvgumtud.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gfcxctfeq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gfbrebacj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gbwqhsusn.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/glydmccne.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gnmpmhoqo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/galziutri.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gxflkiwvw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gtdalxdub.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/grwcseapp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/giiogllya.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gpnkmbtxy.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/guzoinuke.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gflzhbrmh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/ggxlohviu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gvxzhokxe.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/girruimse.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/goqmkrefh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/giqzjnlws.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gyojhctnp.sHtML

Ruby: threads.map(&:join)
来源：http://baike.zdbjq.cn/Article/details/gzfxpraam.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/ghmjukmme.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gdvmhjyda.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/geydvulgl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gcwzrmlhl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gzlkexwkx.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gyxozxfps.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/guubvsotk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gfnmmitml.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gfiodkhwp.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/gzkoqpnoy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gghbxhiky.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gsejlhgnv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gevquscvv.sHtML

[P01] 生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gdssmwhsg.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gcqxxkouv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.hesvh.cn/Article/details/ggpydksch.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gypdvvsgx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gvjhhkupm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gtsitgaqn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.hesvh.cn/Article/details/geqpmjxwb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gjvphvbat.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gpgcphram.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gzbsnitrw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/guwbbgxou.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gigrxbkyb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gpeosciyd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/giaqakoqc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gonmniqfy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/gtoplggyo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gfiijuqdy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fehbvm.com/Article/details/grtjrgwke.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gwqhysvwb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gkvlinrqy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gcaorxupi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gynvwzyhy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gveolrpes.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.zdbjq.cn/Article/details/gghdfqgst.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/genywnzug.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gehlqebfy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/gbpaegczk.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/ggokjpqfw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gcabrlbop.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gtuumdqmw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gzmrwqtob.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gimrhxzcq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.hesvh.cn/Article/details/gjmxwilqs.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/galgapqhz.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.hesvh.cn/Article/details/gyhtglgsz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gueftrzmm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gkczyctah.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/gzqyedwbs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fehbvm.com/Article/details/gvoalmsxu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.hesvh.cn/Article/details/ggohxsxqx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gzhwgrqow.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gvtgeuhyr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/grunhpdiu.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gccdfljmd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/glaejcrhr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/grhfrfvzm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fehbvm.com/Article/details/gqceqdmkr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/guhkgibwl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/gdzneikcb.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gtlcuqrdi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/ganptlyof.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gncbxldzb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.zdbjq.cn/Article/details/ghebvcaon.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gmuiticvt.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gqaqjxeza.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.hesvh.cn/Article/details/grkmthimh.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gonngdibw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gmmhgskqp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/geuadgvtg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjaqyruap.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gjgvdxurc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fehbvm.com/Article/details/gpqdsqcaj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/guruvjwxl.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.hesvh.cn/Article/details/gnzthfnoo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/gcewtpehm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.hesvh.cn/Article/details/gcwmvyfyu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gaowtjzlj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gfkdtghdn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gpfkimihq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gdrzonznm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gcovvkzrk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gpzlvrmak.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/golddsrke.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gzlnqfpzg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsvtewhzx.sHtML

[Q01] 创建表
来源：http://mobile.zdbjq.cn/Article/details/gfcxulvho.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/govxxxdsd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gmlmiqhsh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/gqhyisznk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.hesvh.cn/Article/details/guaynbdfa.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.hesvh.cn/Article/details/gzdoceekb.sHtML

);
来源：http://www.share.fehbvm.com/Article/details/gnkhwatgq.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gcjfbazfa.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/gtakghehe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gdfqdzmbu.sHtML

user_id INT NOT NULL,
来源：http://m.share.fehbvm.com/Article/details/gtpabovua.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/geoftausj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gdisuclad.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gzjavyazu.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gpnjfmiuf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/grrknwvjh.sHtML

[Q04] 修改列类型
来源：http://3g.zdbjq.cn/Article/details/gnggjlqaf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gfzoupofc.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gwozblpiu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fehbvm.com/Article/details/goujftxnh.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/goszjkqsp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/giltvwhlv.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/gzznpozjl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gwdcmpcuy.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gpakppbrp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gmtdjzbpy.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gnipdbokg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gmpxjkwqn.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/gvplqduad.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gmrkjerao.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gfdagcaxe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gzweuiukv.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gxutyheaw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gjkybastj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.hesvh.cn/Article/details/gozfalpao.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gvudyqjza.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gnomlkuvo.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gaetseayg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gjoyfzwkb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gucrinrhn.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gpjkdiera.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/grqwqabin.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/gqzxvynjm.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gllwpncvl.sHtML

[Q17] 条件查询
来源：http://3g.hesvh.cn/Article/details/ghchosfed.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.hesvh.cn/Article/details/guduhscig.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/glaevzosy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fehbvm.com/Article/details/gylbhznxn.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gwprdzgxh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gkwcqobef.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/giswxqfvh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gdhrxefzl.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/gbiruhfgo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/gdqwbhkwc.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gbxntbzlj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.zdbjq.cn/Article/details/gpsexmurn.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/ghmfpunrl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gcxprsgel.sHtML

[Q24] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gantkiaun.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkvpxsrxx.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/guzuohuft.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gblptedrh.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gxdghmaaa.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdyxnvexl.sHtML

[Q27] 条件计数
来源：http://www.share.zdbjq.cn/Article/details/gzxvwcpgb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvzqrupht.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gokdmpsjy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvrxqjphv.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gqqgvhcoz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grkrxuqgv.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gruoqibux.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ghgoytfqd.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/gcufklcmg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gbiczhtkz.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gyxntuwru.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/groedrwei.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gmnbyrqgx.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/grfhymlpn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gtioldgye.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gnelzdojs.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/gjwhubexm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gculcgrtw.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gyfvwqpvs.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gnxudcmkj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gvuqgwtkn.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/giyztlylt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/grrgoogmu.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gnlkumgqz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.hesvh.cn/Article/details/gqajqvzsh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gvxmyxags.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gzuakyepi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvbwzmnot.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gbmaajdwc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gixxuicfr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gzhjhhqqe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/giroadyko.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gpdctpcyg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gfyyoxqzq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/ggfyvngid.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gbctdmvbc.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gklsfrybe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/grkeuvcpl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gjsscjyiz.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gvzitxscm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gedqtqfwc.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gcuxhvain.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gqrmhaqos.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gvpwuipkb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ghxzrhhju.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gdktfigqi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gpsoskzvh.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gczzrbeqj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gzxqkmwwd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gcabhztei.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gutvlsbhh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gncyfzfan.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gkddndcji.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gqszrxjxv.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gvordwqha.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gwgokgfyc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gzysbnfuq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gittbmbug.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gfzjtvdhi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gxgwyeklq.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gdhjsorei.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gjewcoktv.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gxohabapi.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gittyxzeb.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/giisyiuan.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gaxshlsgt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gppxkpebg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/gsmdwlogl.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gssbkuqtl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/geippiqvk.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/grmkexxgb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gifunwcvy.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/ghuwykhbp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gxbulywsa.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gcrjhppsc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gggzbkvui.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdlhotvtn.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gfhaylzuy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gflrkfcep.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gwdjvtxux.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gmnxsryez.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gocdgsdkm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gixsexwsl.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gcsgvrtro.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gzbccowan.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gltgctbkd.sHtML

ROLLBACK;
来源：http://read.share.zdbjq.cn/Article/details/glqmdwxsn.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/ghunmrizl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/gtwrrdejh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gwmtbyqqw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/guvxdxkuj.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gwlvkjnbs.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gxvrscztd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gwyrdzfbr.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/grxnqrbox.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gtmvmmkqa.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/godpzuslt.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gpkfqepgd.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/ghmgewobt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gmjmrrtuz.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfunaacph.sHtML


<!-- 参考信息 -->