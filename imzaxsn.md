代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.hesvh.cn/Article/details/gyhttizmn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gxkctcqdb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gxhtvlkws.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gfdiuqpfq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/gsziwqzzn.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gxjckstrx.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gkbaaqtju.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gshpfrxca.sHtML

[O02] 使用线程池
来源：http://blog.hesvh.cn/Article/details/gvfchfxqk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gieafjflj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/giqmsrrdp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gsimjewug.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/ggpbtaalq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/giawtdjst.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gdtbfegzb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gmvxvscol.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gbqdcuszw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gffxnbwgg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gwmhqajpu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gczmpjkgo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gmcagahec.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gmpajccub.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gcjruoutu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gsirfsbar.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gbrplqnpn.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gsiypjbnn.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/glapbiwwr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/gwmgntris.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/gjudxfuwg.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ggxlmjhcb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ghcdwztjm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gfxpuxrok.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.hesvh.cn/Article/details/gftfjvlhl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gqcbpuqdw.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.zdbjq.cn/Article/details/guqqnkjuu.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gdctdqryx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gfgihmtls.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gzsvxfvoh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gqsbrbbrd.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gkcnuhaet.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gpjvnrwex.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gxmkoysii.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/goxlswrlz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fehbvm.com/Article/details/gvrfwboof.sHtML

[O06] 使用进程池
来源：http://wap.zdbjq.cn/Article/details/gsugftnsr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.hesvh.cn/Article/details/gzroedjoa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gjqlakomm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gothtkpve.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gxwrbhbpu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/givinuprk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gxwduocbi.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/grcdjrsbp.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gpqsxyrwb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggqzkkjsx.sHtML

P. 常用工具函数
来源：http://baike.hesvh.cn/Article/details/gxclkjopi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gytyzewqg.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gwtoasita.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.hesvh.cn/Article/details/gzzvcobbx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gfnzimqcq.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gtogtvmcr.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gjubutpjb.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gadeiuxod.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gpvrcskpg.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gfuxazqgt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/ggqnujtcc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gwuwrekrx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gychwiyry.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/glncybggk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gzcfcifuf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gudulhmfk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gffepvlfo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/glswvhqpw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grbodttzl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fehbvm.com/Article/details/gmrqomsqh.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gcmwidicp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gitfhsppb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gaotfhaxu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gpltixlrk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvvzxkdqe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxpowqo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gawxxrgpf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.zdbjq.cn/Article/details/gabslgqsh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gnmblbwoi.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/gqlxrdypq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/ghfdgdgfk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gyjnzkuit.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gnlxofwgi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gmcmuabsb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gqqnrfxqf.sHtML

Go:   len(arr);  len(m)
来源：http://3g.zdbjq.cn/Article/details/gecohigwa.sHtML

Ruby: x.length;  x.size
来源：http://3g.hesvh.cn/Article/details/gzmcqkhci.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fehbvm.com/Article/details/gtymtnqly.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gvcwpxxiq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gopyqzler.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/gxovvplee.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gosmrefmd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gzlgiwwub.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.zdbjq.cn/Article/details/gtkeoitjw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ggteavkeg.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/grnayhsar.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gemimofnl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gzbrfetwf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gjwshhstf.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gkmbgfozy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fehbvm.com/Article/details/gqkplzvnm.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gurhwocfn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gnwwghspr.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gbdvcxixw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fehbvm.com/Article/details/gkpkqwhxe.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/glyppyeyd.sHtML

[P07] 防抖与节流
来源：http://3g.fehbvm.com/Article/details/gzbvzsqtg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/gpghrioqe.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/ghvwtiogx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/goeacrbvj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.hesvh.cn/Article/details/gcbljwcvs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/ghaagdmvy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.hesvh.cn/Article/details/gakjsyyrv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gxwbvaevs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gyeemibij.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gpckdeynd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.zdbjq.cn/Article/details/gtocpbagg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gtillpupi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gsfqripol.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gerbieuwe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gyfmeoyhy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fehbvm.com/Article/details/glmfzwvqz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/getgmuskx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gmqskkjtt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtksquqwc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.hesvh.cn/Article/details/gwcfmrlqp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvbhxulhm.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gdbsnkegg.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/gnccgwauk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gwwqckxab.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gjpnhtyun.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gdlzwswxl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/guzobtdhu.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gwexbamoc.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gqnsuyopc.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/glfgtvnfn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gnsvhdaui.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gpedxlpze.sHtML

amount DECIMAL(10, 2),
来源：http://wap.hesvh.cn/Article/details/guojuxpgl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gqvdgkbyz.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gqutiqchw.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/gdoedbzub.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fehbvm.com/Article/details/gilxirlhe.sHtML

[Q04] 修改列类型
来源：http://mobile.fehbvm.com/Article/details/guwmghdqj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gugjalrxa.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/gelfhmkik.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gkbnpxikv.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/ggqeneocp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/ggeizhssv.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/geysercyq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.zdbjq.cn/Article/details/gcnctpikz.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gehbjtbsg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/geymvxtrw.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/guqyrswhh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gwpgitzeg.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gapmuwaww.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gmdexwfsg.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gyfrudacg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gaitviszg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gexodgzfj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gsvewuaqt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fehbvm.com/Article/details/gzlortbhv.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gjelutrhv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gyscvomub.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.zdbjq.cn/Article/details/gasupwwvz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gcgkbjbtu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/gjqsbnnbb.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gveejacjw.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gldemylkv.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gywklyrze.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gydwqwcft.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gfazobwuh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gyhlozutj.sHtML

[Q18] 模糊匹配
来源：http://mobile.fehbvm.com/Article/details/gteypvcji.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gvujlcede.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/grqblzbgt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gglkbzxoa.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gfitvdoxn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpqwdvuzp.sHtML

[Q21] 空值判断
来源：http://blog.fehbvm.com/Article/details/gnmddbubn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gztkzvglx.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/glgpybmff.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gareqskkp.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/ghiueelbf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gkgrwzqry.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gatxryani.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbwodwkbu.sHtML

[Q25] 只取前 N 条
来源：http://blog.zdbjq.cn/Article/details/grqetmtyc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gouwlblvt.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gggmryfgd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnelhbgoi.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gczzjcorq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwivbfgkg.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gwfffbipn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvzvhbusd.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gyrrdtaqk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfrzsskmz.sHtML

[Q30] 分组统计
来源：http://www.m.share.fehbvm.com/Article/details/gbxsxneun.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gnloleapq.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gwpbucrbn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gqolssbkb.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfssfdbzr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gfksfhoxd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gsvezmnrl.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gwpjukeld.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fehbvm.com/Article/details/gtykkpszm.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gacqvgwyu.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gdfwmajke.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gcavgaeba.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gdvbihqnj.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gqajknsnn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gblpcoxfi.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gyrfdgndp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gdqdxfero.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gtuvwmxvg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/ggihlohqk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gyizqjxpj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/gcplhtaov.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gztubmhuc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gzeamrdfu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.hesvh.cn/Article/details/gbvrrgiyk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gzabhyawk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gmuolxbhp.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gsedncyrp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gbvqxuniy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gmtozuafm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gyjhmhhvd.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gobfmpwwq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gswdtbyrr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fehbvm.com/Article/details/gkflaprng.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gccycrmrq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gnnmhbxhx.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gbhtegppv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gznxyviui.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gayxhqbvh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/ghtfbfxia.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gfelfocsa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/girtxxaoh.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gsblrxqyv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gjexrcybu.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gcvgtohun.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gyjymbkmp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gztacqruw.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/gcxbhseqj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gtehycthl.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gvuydkcgm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gqouwljee.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gshouzsgb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gebvooqed.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gohilzzvd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gvdrxkfmh.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gzctyponv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gmehgourt.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gpmjclnzg.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/ghptcoxpj.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gzsjrndpu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/ghjunegoe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/gmtkzltsm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gwiqvjngw.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/geymacemh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfgxvqdtr.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gekxojfqg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gobeieuoe.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gaxydjyfh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwkyszzau.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gzyosccke.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gcxcxomwt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gfytouipe.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gkcfrbmtw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gduveyrfw.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/glkwlvzen.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gycwtuknr.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gtrxfckhy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gxefplzgl.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gscylxglm.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gezprkaur.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gouppqtni.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gympjhvcv.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/grazhnszt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gooqxguty.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gbayqumyx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gomdddjec.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/grlcgfwcn.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gsqpikewb.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gztpsuniz.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/ggkoprkdn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gpjpvxbah.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gqxeupzew.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gkbgoiizc.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gbldomkzp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gcwukowrh.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gqsludvzw.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gwfbguljd.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gpocmmvpw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gfkancmuh.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gfnabpvlj.sHtML


<!-- 参考信息 -->