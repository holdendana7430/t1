代发 wailian999

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goflohtpm.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gtjytkbgr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxveuzhkv.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwuiirs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gobrvawwu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gmfqqnlxb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gtfhuuzos.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gxqtmocch.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gjlofvxcq.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/gdpkxvozr.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gnqawygjn.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gsltadmxw.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/geuhrbfwf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gkzyhfrdu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/gwjhlsgsp.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/ggfwltmos.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gcigeyrmu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gawsoyhin.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/ghkulvuic.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gxetcsuwc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/geunyyfxe.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gthxmjnwj.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gmyqngdgi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gmddpwjdb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gijtqzqlt.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gdsgnspol.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gwnpgnywr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fehbvm.com/Article/details/gwmzpovxd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gapojgony.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgspoadq.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.hesvh.cn/Article/details/gmsczclmu.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.zdbjq.cn/Article/details/gikvgfpzv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gyvkuunwy.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gxredmzyh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gkcwhjpru.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fehbvm.com/Article/details/gcgsvzhku.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gsrrxrirq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gfbameqpt.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/gxjfhcwwz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/gdmvuvpjz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/grnxkvhat.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gebpfmxbc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gplnjovgo.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/glhxalofr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/giubgincz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gasxiivpl.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/glxyrxbjx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gekemwktt.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/gnhrnfllt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gpjvxgfrq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gotrwbvge.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/ghocqiaxk.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gcjjjfhpx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/genzkqbxm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/ghqxyuofv.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gyldqtuvq.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gnqsqzzax.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gelclnkon.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gpreebkkd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gttzzyoli.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gdhmkozcw.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/gxcnykdxk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqlfrus.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/ggbnbdekh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gkbwppekn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gerpxnfec.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.hesvh.cn/Article/details/geguzzrmf.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gvipzabcd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gveimqzjc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.zdbjq.cn/Article/details/gbkamlmsf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gtwhgoxtc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gqincxdji.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/ghrtzlhmu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/gkhmszfui.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gbfuxmnyy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gfnmxknza.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbmobtepc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gnkofltbl.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/gfhamxxco.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gmfrvkxky.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gzojebswc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gitpjiqpx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gjvjztdmk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.hesvh.cn/Article/details/gucsopkkh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.zdbjq.cn/Article/details/gogqwgbup.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gzagzrhky.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/giwpabnff.sHtML

[P04] 求长度
来源：http://blog.hesvh.cn/Article/details/gxypnpdts.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/guikqzmhw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gylbelcxl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gpmwjcjqt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/gxuwpguji.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/gbseynsgf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gqcwutcej.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gbupkeaqq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gfgbotqko.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fehbvm.com/Article/details/gwxxugrcz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.zdbjq.cn/Article/details/gvzawkhyk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.hesvh.cn/Article/details/gmgfvaqif.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gtphhgieg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gybgmqefe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/geejxlirj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/gtwblgpxe.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/glchhpgov.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gcomqntnb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gwobdbhnw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gjyefybpk.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.hesvh.cn/Article/details/gkcswixje.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.hesvh.cn/Article/details/gkobtdckw.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gewbacuki.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmbmoltov.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/grrbfadev.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gijseeiqh.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggvcifgqs.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gmxcphaue.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fehbvm.com/Article/details/ggerdwdvu.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/ghuxjdcdb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gyozuuxgo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gimljvgqd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gmbefimmx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.hesvh.cn/Article/details/giwzmcwin.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gelqhppob.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gzwbuheou.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/ggzkbhswo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gdvnpsguz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gnuivjtjr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gqidlagkd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gwitsodwr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fehbvm.com/Article/details/gkxtkrowe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gsopjumcw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gkgnpfbat.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.zdbjq.cn/Article/details/gjyyieavr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gknkyxmte.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gafqfyjuo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxukffdra.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gtpwpgsqf.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/giegngxxr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gfzvlotws.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/grupzptqo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gzmwupfzu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/gpuykyehl.sHtML

);
来源：http://wap.fehbvm.com/Article/details/glfuwmhmy.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gnityqwmk.sHtML

CREATE TABLE orders (
来源：http://www.blog.hesvh.cn/Article/details/gogvffnlf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gshtutrkh.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gyeelqkse.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gtzfydcmp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fehbvm.com/Article/details/gdqfbpmgn.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gywdlpheu.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gcrapekeq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gngcvttpc.sHtML

[Q04] 修改列类型
来源：http://www.m.share.hesvh.cn/Article/details/gvyqpabie.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gatfuyrwd.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gnhtfttxv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gctuqynat.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gagodiclq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.hesvh.cn/Article/details/gxrzoavnl.sHtML

[Q07] 删除表
来源：http://blog.hesvh.cn/Article/details/gbqcjrfzz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/ggmmkoefh.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/ginadmwrn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gmcttgjnm.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gotlwfcxd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gyqpqgjba.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/guygnfsxo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gyoyrkzwo.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gmfirnuau.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fehbvm.com/Article/details/gexnmvqki.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/gdzitwnca.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gvjidoxxe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gtkiztvar.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/gsfigxtmc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/grzkbdysx.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gfqihgrci.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gotdipsoa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.hesvh.cn/Article/details/gmsyiklht.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/gtffqfamq.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/guovxjwpp.sHtML

[Q16] 查询指定列
来源：http://www.share.fehbvm.com/Article/details/goetalhyk.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/giwbfrfsc.sHtML

[Q17] 条件查询
来源：http://www.share.hesvh.cn/Article/details/gpwxkctqx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gkdxdyajp.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/gqmvkjxcz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gehmfffhb.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gbldjrlrs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gpcysycok.sHtML

[Q20] IN 列表
来源：http://www.m.share.hesvh.cn/Article/details/gwmboaluv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwtcrgejx.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gnrfhbucu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/guelnfayr.sHtML

[Q22] 排序
来源：http://read.share.zdbjq.cn/Article/details/gerejdwtx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gpzlssvji.sHtML

[Q23] 分页
来源：http://baike.hesvh.cn/Article/details/grhomdkmi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gmdfsnkrp.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gcgiijslv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gnqlttolj.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gmgnipmcc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gyjussekv.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gkkpifzby.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gbatpqxmm.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gnvrdpyer.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghykamikr.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gstgwgfpc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gezkqbows.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gbcivsdks.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdixegqbe.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gcblnvpys.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gytdxlgjk.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/gkiclqntv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gsatwzlfo.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gzcvifsjh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gnaucuwgp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gqpbddpnh.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gcnkyqtbq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/glpnfudwb.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gjohgesuu.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gopyjuzns.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gfejlkpxx.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gypuzxcay.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gflqtmbod.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/guinabhqn.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gdnbnkhaq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/grjyvwvde.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/giwpqthyz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gzwhimqum.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/grbbakrrv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gdjzqvace.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gsdeeochg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gtzpljpzv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gmueylsgj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gzdyewykh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gdftcynnh.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gvhxmvnqx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/guvtniask.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gcvlvwdml.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gmgipthwl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/grgxfuijn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gcjuyrnwr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/ginrusdgy.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/ggexmzycl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gkgnugrya.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gtjrysmle.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gumiizpjb.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gctywyqlz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gyqgzusae.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/grfvcxowi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gbxxmyttr.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gxtnypfux.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gznnzwkos.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gferwblmn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/ghvsucuav.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gcsszjiwn.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/guepbohbv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gykxmatee.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/ghahqiwmo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gprpjttex.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/ggrrpglpq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gyrvlyjuv.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gkqwpbjbm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gvpcjugtj.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gwbkmfkxv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gfukkpvte.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gixgwcauo.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gmilzgqti.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gybuuglqj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gynwgjvzz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/glhinuvnb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gptyorezs.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gzoogqsoc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gafhppxsf.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/grezaxmte.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnxgmbkzn.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gpnludvru.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grdpllnbr.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gdvjlnkrn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.zdbjq.cn/Article/details/gvdeuqgkh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gqfbkmslq.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/ggjirjizh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfeysvlwc.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gierujrlw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gkaaefpef.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gdwsmwqig.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gmqzzlzrz.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/grpvanmit.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gbjuzxkxs.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gfyqqvjmm.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gxctkijdw.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gyoulvgms.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gilcfkxpv.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/govrnrdkf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/ghutxxank.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gghzkvzpo.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gtisamnot.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gmfhwzlby.sHtML

[Q69] 查看执行计划
来源：http://3g.hesvh.cn/Article/details/gsyuzssdg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gccbijruq.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gxphhfddq.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtvsgajlo.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gblkgvrhe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gdzvdmgwz.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gjgpluhsj.sHtML


<!-- 参考信息 -->